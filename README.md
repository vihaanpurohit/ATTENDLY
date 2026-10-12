# Attendly — General Attendance Tracker 📚

**Know your attendance. Know your limits.**

Attendly is a lightweight, responsive, browser-based attendance tracker designed to help college students monitor their overall and subject-wise attendance. Students can create their own subjects, configure their weekly timetable, record missed classes, and calculate whether they meet their minimum attendance requirements.

The application works offline and stores data locally in the browser, so no account, backend server, or database setup is required.

## ✨ Features

### 📊 Attendance Dashboard

* View overall attendance percentage.
* Monitor subject-wise attendance statistics.
* Identify subjects with critical, warning, or safe attendance levels.
* Calculate how many additional classes you can miss.
* Determine how many consecutive classes you need to attend to reach your target.

### 📚 Subject Management

* Add and manage custom subjects.
* Specify subject codes and types.
* Support Theory, Lab, Practical, and Other categories.
* Track attendance separately for each subject.

### 🗓️ Timetable Management

* Create a custom weekly timetable.
* Set class days, start times, and end times.
* Assign subjects and batches to individual classes.
* Edit or delete timetable entries.
* Import timetable data using CSV files or pasted text.

### ✅ Attendance Recording

* Mark individual classes as attended, missed, or cancelled.
* Enter missed-class counts for faster attendance tracking.
* Add extra classes.
* View attendance records organized by date.

### ⚙️ Settings and Customization

* Configure the semester start date.
* Set the minimum required attendance percentage.
* Configure your batch.
* Switch between light and dark themes.
* Add holidays to exclude them from scheduled attendance calculations.

### 💾 Data Management

* Automatically save data in browser Local Storage.
* Export attendance data as a JSON backup.
* Restore data from a previous JSON backup.
* Reset application data when required.

### 📱 Responsive and Offline-Friendly

* Responsive layout for desktop and mobile screens.
* Mobile-friendly bottom navigation.
* No external libraries or frameworks required.
* Runs locally in a modern web browser without a backend server.

## 🛠️ Technologies Used

* **HTML5** — Application structure.
* **CSS3** — Styling, responsive layouts, and theme customization.
* **Vanilla JavaScript** — Application logic and attendance calculations.
* **Local Storage API** — Persistent browser-based data storage.
* **File API** — CSV import and JSON backup handling.

## 🚀 Getting Started

### Prerequisites

You only need a modern web browser, such as Google Chrome, Microsoft Edge, Firefox, or Safari.

### Run Locally

1. Clone this repository:

   ```bash
   git clone <YOUR_GITHUB_REPOSITORY_URL>
   ```

2. Open the project folder.

3. Open the HTML file in your web browser.

   ```text
   index.html
   ```

   If your uploaded file has a different name, open that HTML file instead.

4. Complete the initial setup:

   * Enter your semester start date.
   * Set your minimum attendance requirement.
   * Add your subjects.
   * Create or import your timetable.
   * Enter your missed-class counts.

5. Start tracking your attendance.

**Note:** You can also download the HTML file and open it directly without installing any dependencies.

## 📥 Importing a Timetable

Attendly supports CSV files and pasted timetable data.

Use the following column format:

```csv
Day,Start,End,Subject,Type,Batch
Monday,09:00,10:00,Mathematics,Theory,All
Tuesday,09:00,11:00,Physics Lab,Lab,A
Wednesday,10:00,11:00,Computer Science,Theory,B
```

### Import Instructions

1. Add or configure your subjects.
2. Open the timetable import option.
3. Select a CSV file or paste timetable rows.
4. Import the data.
5. Review your timetable and make any necessary corrections.

**Important:** Use valid weekday names and 24-hour time values in `HH:MM` format. The application may create a new subject automatically when an imported subject name does not match an existing subject.

## 📈 How Attendance Is Calculated

Attendly calculates attendance using the following formula:

**Attendance Percentage = (Classes Attended ÷ Classes Conducted) × 100**

The application compares the calculated percentage with your configured minimum attendance requirement.

For example, if you attended 36 out of 40 conducted classes:

```text
Attendance = (36 / 40) × 100
           = 90%
```

If your minimum attendance requirement is 75%, your attendance is above the required threshold.

Attendly also estimates:

* The maximum additional classes you can miss while maintaining the required attendance.
* The number of consecutive classes you need to attend to reach the required percentage.

### Attendance Assumption

The quick-count workflow assumes that past scheduled classes were attended unless you record them as missed. You can use individual class corrections for more detailed tracking.

Attendance calculations depend on the accuracy of your timetable, semester start date, holidays, and recorded attendance.

## 💾 Data Storage and Backup

Attendly stores its application data in your browser's Local Storage.

This means:

* Your attendance data stays in the browser where you use the application.
* No account or remote database is required.
* Your data is not automatically synchronized across browsers or devices.
* Clearing browser storage may delete your saved attendance information.

### Create a Backup

1. Open **Settings**.
2. Locate the **Backup** section.
3. Select **Export JSON**.
4. Save the downloaded backup file.

### Restore a Backup

1. Open **Settings**.
2. Select **Import JSON**.
3. Choose a previously exported Attendly backup.
4. Confirm that your information has been restored correctly.

**Recommendation:** Export backups regularly, especially before clearing browser data or switching devices.

## 📂 Project Structure

The project is intentionally simple and does not require a build system.

```text
attendly/
├── index.html
└── README.md
```

The HTML file contains the application's structure, styling, and JavaScript logic in a single file.

If you retain the original uploaded filename, use that filename instead of `index.html`, or rename it to `index.html` before uploading it to your repository.

## 🌐 Deployment

You can publish Attendly using GitHub Pages.

1. Upload the HTML file and `README.md` to your GitHub repository.
2. If necessary, rename the HTML file to `index.html`.
3. Open your repository's **Settings**.
4. Navigate to **Pages**.
5. Select the branch you want to deploy, usually `main`.
6. Select the repository root folder.
7. Save your settings and wait for deployment.

GitHub Pages can host the static application without requiring a backend server.

After deployment, open the published website and verify that attendance data can be saved and restored in your browser.

## ⚠️ Limitations

* Data is stored locally in the browser rather than on a remote server.
* Attendance information does not automatically synchronize across devices.
* Browser storage can be lost if site data is cleared.
* Timetable imports support CSV and text formats; PDF timetable extraction is not implemented.
* Attendance calculations depend on the timetable and records entered by the user.
* The application is intended for personal attendance tracking and does not connect to official college attendance systems.

## 🔮 Future Improvements

Potential enhancements include:

* Cloud synchronization and user authentication.
* Downloadable attendance reports.
* Attendance trend charts and monthly summaries.
* Notifications for attendance thresholds.
* Improved timetable import and validation.
* Multi-semester attendance history.
* Additional export formats.

## 🤝 Contributing

Contributions, bug reports, and feature suggestions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Make your changes.
4. Test the application in a modern browser.
5. Submit a pull request describing your changes.

## 📄 License

No license is specified in the original project file.

Before distributing or modifying the project publicly, consider adding a suitable license to clarify how others may use, modify, and redistribute the code.

---

**Attendly — Know your attendance. Know your limits.**
