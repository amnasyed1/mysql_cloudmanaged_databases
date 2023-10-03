
CREATE TABLE doctors (
    doctor_id INT PRIMARY KEY AUTO_INCREMENT,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    specialization VARCHAR(50) DEFAULT 'General Practice'
);

CREATE TABLE patients (
    patient_id INT PRIMARY KEY AUTO_INCREMENT,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    date_of_birth DATE,
    primary_doctor_id INT,
    FOREIGN KEY (primary_doctor_id) REFERENCES doctors(doctor_id)
);

CREATE TABLE demographics (
    demographic_id INT PRIMARY KEY AUTO_INCREMENT,
    patient_id INT UNIQUE,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    date_of_birth DATE,
    address TEXT,
    phone_number VARCHAR(15),
    email VARCHAR(100),
    FOREIGN KEY (patient_id) REFERENCES patients(patient_id)
);

CREATE TABLE medications (
    medication_id INT PRIMARY KEY AUTO_INCREMENT,
    medication_name VARCHAR(100) NOT NULL
);

CREATE TABLE patient_medications (
    patient_medication_id INT PRIMARY KEY AUTO_INCREMENT,
    patient_id INT,
    medication_id INT,
    prescribed_date DATE NOT NULL,
    FOREIGN KEY (patient_id) REFERENCES patients(patient_id),
    FOREIGN KEY (medication_id) REFERENCES medications(medication_id)
);

CREATE TABLE allergies (
	patient_allergy_id INT PRIMARY KEY AUTO_INCREMENT,
    patient_medication_allergy_name VARCHAR(50) NOT NULL,
    patinet_food_allergy_name VARCHAR(50) NOT NULL,
    patient_id INT,
    FOREIGN KEY (patient_id) REFERENCES patients(patient_id)
);

select *
from doctors;
select * 
from patients;
select *
from demographics;
select * 
from medications;
select * 
from patient_medications;
select *
from allergies;
