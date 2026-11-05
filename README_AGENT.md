# Agent Task: Rebuild Demo Data Based on SPM Additional Mathematics Syllabus

## Current Project
You are working directly inside the real project folder:

D:\Y3S2\E-LearningApp

This is a Secondary Math E-Learning App with teacher, student, classroom, quiz, community feed, and VQA tutor modules.

## Main Goal
The previous demo data was too generic and placeholder-based. Remove or replace the previous generic demo seed data and rebuild the demo dataset so it is consistent with:

1. The current system implementation and database schema.
2. The existing app modules and screens.
3. The SPM / KSSM Additional Mathematics Form 4 and Form 5 syllabus.
4. Realistic FYP demonstration flow.

## Important Rules

1. First inspect the existing database schema, Supabase files, frontend screens, backend routes, and existing seed files.
2. Do not assume table names. Match the actual schema used by this project.
3. Remove or replace the previous generic demo data created earlier.
4. Make the new seed script idempotent:
   - Running it multiple times should not create duplicate records.
   - Use fixed demo IDs, fixed demo emails, or cleanup logic before inserting.
5. Do not modify unrelated UI.
6. Do not hardcode practice data directly into screens if the database already supports it.
7. Do not expose or modify real `.env` secrets.
8. Do not copy textbook questions word-for-word. Generate original practice questions aligned with the syllabus topics.
9. If the database does not support a certain field, adapt the data to the closest existing field instead of forcing a large schema change.
10. Only add schema columns/tables if absolutely necessary and if it is safe for the current implementation.

## Required Output

Create or update one proper seed implementation:

- `supabase/seed_demo.sql`, or
- `scripts/seedDemo.ts`, or
- the existing backend seed mechanism, depending on the current project structure.

Also update the project README with:

- how to run the seed script,
- demo login accounts,
- demo classroom structure,
- demo presentation flow,
- warning that this is fake demo data only.

---

# Syllabus-Aligned Demo Data Structure

## Form 4 Additional Mathematics Chapters

Create chapter/topic data for Form 4:

1. Functions
   - Functions
   - Composite Functions
   - Inverse Functions

2. Quadratic Functions
   - Quadratic Equations and Inequalities
   - Types of Roots of Quadratic Equations
   - Quadratic Functions

3. Systems of Equations
   - Systems of Linear Equations in Three Variables
   - Simultaneous Equations involving One Linear Equation and One Non-Linear Equation

4. Indices, Surds and Logarithms
   - Laws of Indices
   - Laws of Surds
   - Laws of Logarithms
   - Applications of Indices, Surds and Logarithms

5. Progressions
   - Arithmetic Progressions
   - Geometric Progressions

6. Linear Law
   - Linear and Non-Linear Relations
   - Linear Law and Non-Linear Relations
   - Applications of Linear Law

7. Coordinate Geometry
   - Divisor of a Line Segment
   - Parallel Lines and Perpendicular Lines
   - Areas of Polygons
   - Equations of Loci

8. Vectors
   - Vectors
   - Addition and Subtraction of Vectors
   - Vectors in a Cartesian Plane

9. Solution of Triangles
   - Sine Rule
   - Cosine Rule
   - Area of a Triangle
   - Application of Sine Rule, Cosine Rule and Area of a Triangle

10. Index Number
   - Index Numbers
   - Composite Index

## Form 5 Additional Mathematics Chapters

Create chapter/topic data for Form 5:

1. Circular Measure
   - Radian
   - Arc Length of a Circle
   - Area of Sector of a Circle
   - Application of Circular Measures

2. Differentiation
   - Limit and its Relation to Differentiation
   - The First Derivative
   - The Second Derivative
   - Application of Differentiation

3. Integration
   - Integration as the Inverse of Differentiation
   - Indefinite Integral
   - Definite Integral
   - Application of Integration

4. Permutation and Combination
   - Permutation
   - Combination

5. Probability Distribution
   - Random Variable
   - Binomial Distribution
   - Normal Distribution

6. Trigonometric Functions
   - Positive Angles and Negative Angles
   - Trigonometric Ratios of any Angle
   - Graphs of Sine, Cosine and Tangent Functions
   - Basic Identities
   - Addition Formulae and Double Angle Formulae
   - Application of Trigonometric Functions

7. Linear Programming
   - Linear Programming Model
   - Application of Linear Programming

8. Kinematics of Linear Motion
   - Displacement, Velocity and Acceleration as a Function of Time
   - Differentiation in Kinematics of Linear Motion
   - Integration in Kinematics of Linear Motion
   - Application of Kinematics of Linear Motion

---

# Demo Users

Create realistic fake demo users.

## Teachers

1. Ms. Tan Mei Ling
   - Role: Teacher
   - Focus: Form 4 Additional Mathematics

2. Mr. Ahmad Hafiz
   - Role: Teacher
   - Focus: Form 5 Additional Mathematics

## Students

Create 12 students with Malaysian-style names.

Suggested names:

1. Jason Ng
2. Nur Aisyah
3. Tan Wei Jun
4. Siti Nurhaliza
5. Lim Jia En
6. Muhammad Danish
7. Chong Kai Xin
8. Arif Hakimi
9. Priya Nair
10. Lee Xin Yi
11. Amirul Syafiq
12. Wong Zhi Hao

Assign students across Form 4 and Form 5 classrooms.

---

# Demo Classrooms

Create at least these classrooms:

1. Form 4 Add Maths - Core Foundations
   - Teacher: Ms. Tan Mei Ling
   - Main chapters:
     - Functions
     - Quadratic Functions
     - Indices, Surds and Logarithms
     - Progressions

2. Form 4 Add Maths - Geometry and Vectors
   - Teacher: Ms. Tan Mei Ling
   - Main chapters:
     - Coordinate Geometry
     - Vectors
     - Solution of Triangles

3. Form 5 Add Maths - Calculus and Circular Measure
   - Teacher: Mr. Ahmad Hafiz
   - Main chapters:
     - Circular Measure
     - Differentiation
     - Integration
     - Kinematics of Linear Motion

4. Form 5 Add Maths - Probability and Trigonometry
   - Teacher: Mr. Ahmad Hafiz
   - Main chapters:
     - Permutation and Combination
     - Probability Distribution
     - Trigonometric Functions
     - Linear Programming

---

# Quiz Requirements

Create quizzes that are aligned with the chapters above.

Each quiz should contain:

- title
- form level
- chapter
- subtopic
- difficulty
- assigned classroom
- due date
- 5 to 8 original questions
- multiple-choice options if the current system supports MCQ
- correct answer
- explanation or solution steps if the current system supports explanations

## Required Quizzes

Create at least 12 quizzes:

### Form 4 Quizzes

1. Functions and Mapping Practice
   - Chapter: Functions
   - Include questions about function notation, image/object, domain/range, vertical line test.

2. Composite and Inverse Functions
   - Chapter: Functions
   - Include composite function and inverse function practice.

3. Quadratic Equations and Roots
   - Chapter: Quadratic Functions
   - Include discriminant, roots, factorisation, and graph interpretation.

4. Indices, Surds and Logarithms Review
   - Chapter: Indices, Surds and Logarithms
   - Include laws of indices, simplifying surds, logarithm laws, and applications.

5. Arithmetic and Geometric Progressions
   - Chapter: Progressions
   - Include nth term, sum of AP, sum of GP, and sum to infinity.

6. Coordinate Geometry and Vectors
   - Chapter: Coordinate Geometry / Vectors
   - Include midpoint/divisor, gradient, perpendicular lines, vector magnitude, and vector addition.

7. Solution of Triangles
   - Chapter: Solution of Triangles
   - Include sine rule, cosine rule, area formula, and real-world triangle applications.

8. Index Number and Composite Index
   - Chapter: Index Number
   - Include simple index number and weighted composite index.

### Form 5 Quizzes

9. Circular Measure Basics
   - Chapter: Circular Measure
   - Include radians, degree conversion, arc length, and sector area.

10. Differentiation Fundamentals
   - Chapter: Differentiation
   - Include limits, first derivative, tangent gradient, and second derivative.

11. Integration Fundamentals
   - Chapter: Integration
   - Include indefinite integrals, definite integrals, area under curve, and volume concept if supported.

12. Probability and Normal Distribution
   - Chapter: Probability Distribution
   - Include random variables, binomial distribution, mean, standard deviation, and normal distribution basics.

13. Trigonometric Functions and Identities
   - Chapter: Trigonometric Functions
   - Include graph features, identities, double angle formula, and angle signs.

14. Linear Programming and Kinematics
   - Chapter: Linear Programming / Kinematics
   - Include constraints, feasible region, objective function, displacement, velocity, and acceleration.

---

# Community Feed Demo Data

Create realistic community posts connected to the same syllabus topics.

Create at least 15 posts.

Each post should include:

- student author
- chapter/topic
- question title
- question body
- solved or unsolved status
- comments
- at least 5 posts with teacher verified answers
- at least 3 posts that mention image-based questions for VQA demo

Suggested post examples:

1. "How do I know whether a relation is a function?"
   - Topic: Form 4 Functions

2. "Confused about composite function order fg(x) and gf(x)"
   - Topic: Form 4 Functions

3. "Why does the discriminant decide the type of roots?"
   - Topic: Form 4 Quadratic Functions

4. "Need help simplifying surds with conjugates"
   - Topic: Form 4 Indices, Surds and Logarithms

5. "How to identify common ratio in geometric progression?"
   - Topic: Form 4 Progressions

6. "How to use sine rule when two angles are given?"
   - Topic: Form 4 Solution of Triangles

7. "How to convert 150 degrees into radians?"
   - Topic: Form 5 Circular Measure

8. "Why is dy/dx the gradient of tangent?"
   - Topic: Form 5 Differentiation

9. "How to decide the limits for area under curve?"
   - Topic: Form 5 Integration

10. "Permutation or combination?"
   - Topic: Form 5 Permutation and Combination

11. "How do I know when to use binomial distribution?"
   - Topic: Form 5 Probability Distribution

12. "Confused about sine graph amplitude and period"
   - Topic: Form 5 Trigonometric Functions

13. "How to shade the feasible region?"
   - Topic: Form 5 Linear Programming

14. "Velocity vs acceleration in kinematics"
   - Topic: Form 5 Kinematics

15. "Can the VQA tutor solve a handwritten circular measure diagram?"
   - Topic: VQA / Circular Measure

---

# VQA Demo Data

If the system supports VQA history, create 6 sample VQA records.

Each should include:

- student
- form level
- chapter
- image prompt or placeholder image path
- detected question summary
- step-by-step AI response
- confidence note
- limitation note if needed

Suggested VQA records:

1. Form 4 Functions
   - Image description: arrow diagram mapping set X to set Y
   - AI response: explains whether it is a function and identifies domain/range.

2. Form 4 Quadratic Functions
   - Image description: graph of a parabola
   - AI response: identifies turning point, axis of symmetry, and roots.

3. Form 4 Solution of Triangles
   - Image description: triangle with two sides and included angle
   - AI response: suggests cosine rule.

4. Form 5 Circular Measure
   - Image description: sector with radius and angle in radians
   - AI response: calculates arc length and sector area.

5. Form 5 Differentiation
   - Image description: curve with tangent at a point
   - AI response: explains gradient and derivative.

6. Form 5 Linear Programming
   - Image description: graph with shaded feasible region
   - AI response: explains constraints and objective function.

---

# Student Attempt Data

Create attempt records so teacher dashboards look meaningful.

Include mixed performance:

- high-performing students
- average students
- weak students
- pending attempts
- recently submitted attempts

Suggested score distribution:

- 3 students: 80–100%
- 5 students: 50–79%
- 3 students: 20–49%
- 1–2 students: pending or not attempted

Make sure the attempt records match the existing quiz/question schema.

---

# Required Demo Flow

The final seed data must support this presentation flow:

1. Login as teacher.
2. View Form 4 and Form 5 classrooms.
3. Open classroom details.
4. View syllabus-aligned quizzes.
5. View student attempts/performance.
6. Open community feed.
7. See posts grouped by Additional Mathematics topics.
8. View teacher verified answers.
9. Login as student.
10. View assigned quizzes.
11. Attempt a quiz.
12. View community posts.
13. Open VQA tutor page.
14. Show VQA history or sample AI tutoring interaction.

---

# Cleanup Requirement

Before inserting new syllabus-aligned data:

1. Find the previous generic demo data.
2. Remove or replace it safely.
3. Avoid deleting real user data.
4. Prefer deleting only records with demo emails, demo IDs, demo classroom names, or demo-specific markers.
5. Add comments in the seed file explaining which section cleans previous demo data.

---

# Final Response Required From Agent

After implementation, report:

1. Files created.
2. Files modified.
3. How to run the seed script.
4. Demo accounts created.
5. Any schema assumptions made.
6. Any parts that could not be implemented because the current schema does not support them.