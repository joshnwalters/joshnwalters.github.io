---
layout: project
type: project
image: images/ts_logo.png
title: PillPal
permalink: projects/PillPal
# All dates must be YYYY-MM-DD format!
date: 2020-02-23
labels:
  - Java
  - Spring Framework
  - SQL
  - Android/iOS
summary: An all inclusive medical informatics application that streamlines interaction between patients, doctors, and pharmacists.
---


PillPal is an app inspired by my wife's career as a pharmacist. Currently she and the other pharmacists on her staff make numerous phone calls to patients and doctors in order to refill prescriptions.

PillPal will have three user types. The first is the patient. Using a mobile app, the patient will be able to view what drugs they are currently prescribd, and set reminders to take said drugs. Each time the user clicks the notification that they have taken the drug, an amount of drug remaining field in the database will subtract the dosage. Once this amount gets below a certain threshold, a notification will be sent to the doctor to renew prescription.

The second user type is the doctor. The doctor can use the app to write prescriptions, and communicate any pertinent information to the patient. I am currently unsure as to how the prescription writing process is performed, but I would like this to be automated, so the doctor writes script in app, then it is automatically sent to the patient's pharmacy of their choosing. Additional functionality would be warnings based on drug interactions or dosings.

The final user type would be the pharmacy. The pharmacy will receive the prescriptions, then based on the queue at the pharmacy, will send a notification to the user informing them of the estimated time the script will be filled.


I would like this app to be as agnostic as possible. By this I mean I don't want it to work solely on one OS, and I don't want it tailored to any one pharmacy, say CVS or Walgreen's. The target demographic is anyone who writes prescriptions and any pharmacy. Drug stores would be whom the app would be marketed toward. These stores would have the most to gain, as it wold greatly increase their productivity. Doctors and patients would be the most difficult entities to market the app to.
