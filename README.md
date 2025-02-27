# -----------------------------------------
# CUSTOMER CLASS
# -----------------------------------------
class Customer:
    """
    Represents a customer in the delivery management system.
    """

    def __init__(self, customer_id="", first_name="", last_name="", email="", address="", phone_number=""):
        """
        Constructor for Customer.
        Initializes all private attributes with optional default values.
        """
        self.__customer_id = customer_id
        self.__first_name = first_name
        self.__last_name = last_name
        self.__email = email
        self.__address = address
        self.__phone_number = phone_number

    # -----------------------
    # Getters and Setters
    # -----------------------
    def setCustomer_id(self, customer_id):
        """Sets the customer's ID."""
        self.__customer_id = customer_id

    def getCustomer_id(self):
        """Returns the customer's ID."""
        return self.__customer_id

    def setFirst_name(self, first_name):
        """Sets the customer's first name."""
        self.__first_name = first_name

    def getFirst_name(self):
        """Returns the customer's first name."""
        return self.__first_name

    def setLast_name(self, last_name):
        """Sets the customer's last name."""
        self.__last_name = last_name

    def getLast_name(self):
        """Returns the customer's last name."""
        return self.__last_name

    def setEmail(self, email):
        """Sets the customer's email."""
        self.__email = email

    def getEmail(self):
        """Returns the customer's email."""
        return self.__email

    def setAddress(self, address):
        """Sets the customer's address."""
        self.__address = address

    def getAddress(self):
        """Returns the customer's address."""
        return self.__address

    def setPhone_number(self, phone_number):
        """Sets the customer's phone number."""
        self.__phone_number = phone_number

    def getPhone_number(self):
        """Returns the customer's phone number."""
        return self.__phone_number

    # -----------------------
    # Additional Methods
    # -----------------------
    def placeOrder(self, order_details):
        """Simulates placing an order with given details."""
        print(f"Customer {self.__customer_id} placed an order: {order_details}")

    def trackOrder(self, order_id):
        """Simulates tracking an existing order by order ID."""
        print(f"Customer {self.__customer_id} is tracking order {order_id}.")

    def cancelOrder(self, order_id):
        """Simulates canceling an existing order by order ID."""
        print(f"Customer {self.__customer_id} canceled order {order_id}.")

    def displayCustomer_info(self):
        """Displays the customer's complete information."""
        info = (
            f"Customer ID: {self.__customer_id}\n"
            f"Name: {self.__first_name} {self.__last_name}\n"
            f"Email: {self.__email}\n"
            f"Address: {self.__address}\n"
            f"Phone Number: {self.__phone_number}\n"
        )
        print(info)


# -----------------------------------------
# ADMIN CLASS
# -----------------------------------------
class Admin:
    """
    Represents an admin user in the delivery management system.
    """

    def __init__(self, admin_id="", first_name="", last_name="", email="", role=""):
        """
        Constructor for Admin.
        Initializes all private attributes with optional default values.
        """
        self.__admin_id = admin_id
        self.__first_name = first_name
        self.__last_name = last_name
        self.__email = email
        self.__role = role

    # -----------------------
    # Getters and Setters
    # -----------------------
    def setAdmin_id(self, admin_id):
        """Sets the admin's ID."""
        self.__admin_id = admin_id

    def getAdmin_id(self):
        """Returns the admin's ID."""
        return self.__admin_id

    def setFirst_name(self, first_name):
        """Sets the admin's first name."""
        self.__first_name = first_name

    def getFirst_name(self):
        """Returns the admin's first name."""
        return self.__first_name

    def setLast_name(self, last_name):
        """Sets the admin's last name."""
        self.__last_name = last_name

    def getLast_name(self):
        """Returns the admin's last name."""
        return self.__last_name

    def setEmail(self, email):
        """Sets the admin's email."""
        self.__email = email

    def getEmail(self):
        """Returns the admin's email."""
        return self.__email

    def setRole(self, role):
        """Sets the admin's role."""
        self.__role = role

    def getRole(self):
        """Returns the admin's role."""
        return self.__role

    # -----------------------
    # Additional Methods
    # -----------------------
    def manageUsers(self):
        """Simulates managing users in the system."""
        print(f"Admin {self.__admin_id} is managing users.")

    def generateReports(self):
        """Simulates generating system reports."""
        print(f"Admin {self.__admin_id} generated reports.")

    def assignDelivery(self, order_id, staff_id):
        """Simulates assigning a delivery to a delivery staff."""
        print(f"Admin {self.__admin_id} assigned order {order_id} to staff {staff_id}.")

    def displayAdmin_info(self):
        """Displays the admin's complete information."""
        info = (
            f"Admin ID: {self.__admin_id}\n"
            f"Name: {self.__first_name} {self.__last_name}\n"
            f"Email: {self.__email}\n"
            f"Role: {self.__role}\n"
        )
        print(info)


# -----------------------------------------
# DELIVERY STAFF CLASS
# -----------------------------------------
class DeliveryStaff:
    """
    Represents a delivery staff member in the delivery management system.
    """

    def __init__(self, staff_id="", first_name="", last_name="", phone_number="", vehicle_type=""):
        """
        Constructor for DeliveryStaff.
        Initializes all private attributes with optional default values.
        """
        self.__staff_id = staff_id
        self.__first_name = first_name
        self.__last_name = last_name
        self.__phone_number = phone_number
        self.__vehicle_type = vehicle_type

    # -----------------------
    # Getters and Setters
    # -----------------------
    def setStaff_id(self, staff_id):
        """Sets the staff member's ID."""
        self.__staff_id = staff_id

    def getStaff_id(self):
        """Returns the staff member's ID."""
        return self.__staff_id

    def setFirst_name(self, first_name):
        """Sets the staff member's first name."""
        self.__first_name = first_name

    def getFirst_name(self):
        """Returns the staff member's first name."""
        return self.__first_name

    def setLast_name(self, last_name):
        """Sets the staff member's last name."""
        self.__last_name = last_name

    def getLast_name(self):
        """Returns the staff member's last name."""
        return self.__last_name

    def setPhone_number(self, phone_number):
        """Sets the staff member's phone number."""
        self.__phone_number = phone_number

    def getPhone_number(self):
        """Returns the staff member's phone number."""
        return self.__phone_number

    def setVehicle_type(self, vehicle_type):
        """Sets the type of vehicle used for deliveries."""
        self.__vehicle_type = vehicle_type

    def getVehicle_type(self):
        """Returns the type of vehicle used for deliveries."""
        return self.__vehicle_type

    # -----------------------
    # Additional Methods
    # -----------------------
    def acceptDelivery(self, order_id):
        """Simulates accepting a delivery for a given order ID."""
        print(f"Delivery Staff {self.__staff_id} accepted delivery for order {order_id}.")

    def updateDelivery_status(self, order_id, status):
        """Simulates updating the delivery status of a given order."""
        print(f"Delivery Staff {self.__staff_id} updated order {order_id} status to '{status}'.")

    def reportIssue(self, order_id, issue):
        """Simulates reporting an issue for a given order."""
        print(f"Delivery Staff {self.__staff_id} reported an issue for order {order_id}: {issue}")

    def displayDeliveryStaff_info(self):
        """Displays the delivery staff's complete information."""
        info = (
            f"Staff ID: {self.__staff_id}\n"
            f"Name: {self.__first_name} {self.__last_name}\n"
            f"Phone Number: {self.__phone_number}\n"
            f"Vehicle Type: {self.__vehicle_type}\n"
        )
        print(info)


# -----------------------------------------
# CREATING TWO OBJECTS FOR EACH CLASS
# -----------------------------------------

# 1) Creating two Customer objects
customer1 = Customer("C001", "Alice", "Smith", "alice@example.com", "123 Main St", "555-1234")
customer2 = Customer("C002", "Bob", "Johnson", "bob@example.com", "456 Park Ave", "555-5678")

# Demonstrating some Customer methods
customer1.displayCustomer_info()
customer1.placeOrder("Pizza and Soda")
customer2.displayCustomer_info()
customer2.trackOrder("O1002")

print("--------------------------------------------------")

# 2) Creating two Admin objects
admin1 = Admin("A001", "John", "Doe", "john@example.com", "Manager")
admin2 = Admin("A002", "Jane", "Miller", "jane@example.com", "Supervisor")

# Demonstrating some Admin methods
admin1.displayAdmin_info()
admin1.generateReports()
admin2.displayAdmin_info()
admin2.assignDelivery("O1002", "S001")

print("--------------------------------------------------")

# 3) Creating two DeliveryStaff objects
staff1 = DeliveryStaff("S001", "Mike", "Brown", "555-9999", "Bike")
staff2 = DeliveryStaff("S002", "Emily", "Clark", "555-8888", "Car")

# Demonstrating some DeliveryStaff methods
staff1.displayDeliveryStaff_info()
staff1.acceptDelivery("O1002")
staff2.displayDeliveryStaff_info()
staff2.updateDelivery_status("O1003", "Delivered")
