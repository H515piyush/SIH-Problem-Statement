# Smart India Hackathon Workshop

# Date: 26-10-2026

# Register Number: 212225040482

# Name: Piyush kumar

# Problem Title
SIH 1710: AI-Powered Automated Coach Cleanliness Inspection and Real-Time Feedback System

# Problem Description
Background: Maintaining high standards of hygiene and cleanliness across thousands of long-distance passenger coaches is a major operational challenge for Indian Railways. Manual inspection processes conducted during depot halts or turnaround times are time-consuming, prone to human subjectivity, and lack standardized photographic audit trails. Unaddressed cleanliness issues in coach interiors, lavatories, and doorways often result in passenger dissatisfaction and delayed corrective action.

Description: The problem involves designing an automated, computer-vision-driven cleanliness monitoring system for passenger railway coaches. The solution must capture visual data using stationary inspection arches at washing pits/depots, handheld inspection devices, or onboard IoT cameras. Machine learning models must analyze images and video feeds to detect dirt, accumulated litter, bio-toilet overflow, water logging, and unwashed berths. The platform should auto-grade coaches, flag critical hygiene failures, generate digital job cards for onboard housekeeping staff (OBHS), and allow passengers to report and verify cleanliness status in real time.

Expected Solution: An integrated AI-powered cleanliness auditing platform that includes:

Deep learning computer vision pipeline to detect waste, stains, and unhygienic conditions inside coaches and toilets.

Mobile application for depot inspectors and Onboard Housekeeping Staff (OBHS) to receive automated work orders and upload post-cleaning proofs.

Central administrative dashboard for railway authorities with automated cleanliness scoring, depot rankings, and predictive maintenance alerts.

Passenger feedback interface integrated with PNR/UTS to report unclean zones with geotagged and timestamped photo validation.

# Problem Creator's Organization
Ministry of Railways (in collaboration with Railway Board & CRIS)

# Idea
To develop an automated visual inspection and incident management system that uses edge AI and computer vision to inspect coach interiors, assign an objective cleanliness score, and instantly dispatch maintenance alerts to housekeeping teams.

# Proposed Solution / Architecture Diagram

<img width="860" height="556" alt="Screenshot 2026-10-27 151307" src="https://github.com/user-attachments/assets/2536e027-baa0-4267-b1d1-b958ff3153e5" />


# Use Cases
<img width="877" height="542" alt="image" src="https://github.com/user-attachments/assets/ff8c81dc-12c1-48cf-8c80-ab51dd586794" />

Automated post-trip cleanliness scoring when coaches enter the wash pit or depot.

Automatic detection of litter, discarded bottles, spilled liquids, and dirty washbasins using computer vision.

Auto-generation of targeted digital task lists (job cards) for Onboard Housekeeping Staff (OBHS) with exact coach and berth coordinates.

Passenger self-reporting portal where passengers upload photos of dirty coaches, with AI verifying the validity of the complaint before dispatching staff.

Post-cleaning validation requiring staff to submit an updated photo that the AI compares against the defect image before closing the ticket.

Depot-level and zonal performance benchmarking based on historical cleanliness metrics.

Emergency alerts for severe bio-toilet blockage or water tank depletion.

# Technology Stack
Frontend / Dashboard: React.js, Tailwind CSS, Chart.js

Mobile Application: Flutter (Cross-platform for Android and iOS)

Computer Vision / AI: Python, PyTorch, YOLOv8 / YOLOv11 (custom-trained for train interior debris and stain detection), OpenCV

Backend: Python with FastAPI or Django REST Framework

Message Broker & Task Queue: Celery with Redis / RabbitMQ

Database: PostgreSQL (structured metadata and scores) and MinIO / AWS S3 (secure image/video asset storage)

Edge Deployment: NVIDIA Jetson Nano or Raspberry Pi 4 (for on-depot edge processing)

Tools: VS Code, Docker, Git, and GitHub

# Dependencies
Python 3.10+ runtime environment

PyTorch and CUDA drivers for accelerated deep learning inference

Pre-labeled datasets of railway coach interiors, seats, floor stains, and lavatories

FastAPI or Django REST Framework

PostgreSQL database instance

Object storage bucket (MinIO or S3) for audit-trail photography

Network connectivity (Wi-Fi/4G/5G) at yard maintenance depots and station halts

Flutter SDK for mobile app deployment on rugged handheld devices

Smartphone camera or fixed depot camera rigs with adequate lighting infrastructure
