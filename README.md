🏢 Employee Management System (EMS)
A robust backend API built with Django and PostgreSQL to streamline human resource operations. This system manages employee lifecycles, department hierarchies, and payroll tracking efficiently.

🚀 Key Features
Employee Records: Full CRUD functionality for managing employee profiles (hiring date, position, contact info).

Department Management: Organizes the workforce into structured departments with designated managers.

Payroll System: Tracks salary history, bonuses, and payment statuses for each employee.

Role-Based Access: Secure authentication to ensure only authorized HR personnel can modify sensitive data.

Optimized Queries: Uses Django's select_related and prefetch_related to handle complex database joins with high performance.

🛠️ Tech Stack
Language: Python 3.x

Framework: Django / Django REST Framework

Database: PostgreSQL

Authentication: JWT (JSON Web Tokens) / Token-based

🔧 Installation & Setup
1. Clone the repository:
   git clone https://github.com/naazriin/employee_management.git

   cd employee_management
2. Create a virtual environment:
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
3. Install dependencies:
   pip install -r requirements.txt
4. Database Setup:
   Configure your PostgreSQL credentials in settings.py and run migrations:
   python manage.py makemigrations
   python manage.py migrate
5. Run the server:
   python manage.py runserver

   🛰️ API Endpoints (Quick Look)
GET /api/employees/ - List all employees

POST /api/employees/create/ - Add a new employee

GET /api/departments/ - View department structures

PATCH /api/payroll/{id}/ - Update salary details
