TrackTracker Single-Page Application (TT SPA)
=============================================

Ohio Track Events - Middle School (2026)
----------------------------------------
This web app (SPA with HTML/JS/CSS) assists in tracking Ohio track and field events.

| Event # | Girls Event                         | Event # | Boys Event                           |
|:-------:|:------------------------------------|:-------:|:-------------------------------------|
| 1       | Relay - 4x800 meters                | 2       | Relay - 4x800 meters                 |
| 3       | Hurdles - 100 meters (33" high)     | 4       | High Hurdles - 110 meters (39" high) |
| 5       | Dash - 100 meters                   | 6       | Dash - 100 meters                    |
| 7       | Relay - 4x200 meters**              | 8       | Relay - 4x200 meters**               |
| 9       | Run - 1600 meters                   | 10      | Run - 1600 meters                    |
| 11      | Relay - 4x100 meters**              | 12      | Relay - 4x100 meters**               |
| 13      | Dash - 400 meters #                 | 14      | Dash - 400 meters #                  |
| 15      | Low Hurdles - 300 meters (30" high) | 16      | Hurdles - 300 meters (36" high)      |
| 17      | Run - 800 meters                    | 18      | Run - 800 meters                     |
| 19      | Dash - 200 meters* #                | 20      | Dash - 200 meters* #                 |
| 21      | Relay - 4x400 meters*               | 22      | Relay - 4x400 meters*                |

### Notes/Symbols
1. `* The first heat of the girls 4x400 relay may begin not earlier than 20 minutes after the start of the first heat of the girls 200M when the 3,200 is not being contested in its normal order and when athletes are competing in both events.`
2. `** The first heat of the girls 4 x 100M Relay may begin not earlier than 15 minutes after the start of the first heat of the girls 4x200M Relay when the 1,600 is not being contested in its normal order and when athletes are competing in both events.`
3. `# The first heat of the girls 200M may begin no earlier than 15 min after the start of the first heat of the girls 400M dash anytime the 800M is not competed in its normal order and when athletes are competing in both events.`

### Events of Interest
* Event #8 - Leg #3
* Event #14 - 
* Event #22 - Leg #1

Ohio Field Events - Middle School (2026)
----------------------------------------
* Order is optional!

| Girls Field Event             | Boys Field Event               |
|:------------------------------|:-------------------------------|
| Discus (1K) (2 lbs. 3.27 oz.) | Discus (1.6K) (3 lbs. 8.5 oz.) |
| High Jump                     | High Jump                      |
| Long Jump                     | Long Jump                      |
| Shot Put (4K) (8 lbs. 13 oz.) | Shot Put (5.4K) (12 lbs.)      |

### Events of Interest
* NONE

## Key SPA Goals
I need a webpage to enable a seasonal track meet tracker (i.e., TrackTracker).

### Technical Requirements
* Single self-contained .html file (no external dependencies, pure HTML/CSS/JavaScript SPA)
* Full offline functionality with LocalStorage persistence
* JSON import/export for data portability and backup
* Mobile-responsive design (works on phones, tablets, desktops)
* No build process required (can be used directly in any browser)

### Core Purpose
* Track season-long performance records for athletes in Ohio track and field events (2026 format)
* Support use by coaches, athletes, and record keepers
* Enable historical performance monitoring and personal record (PR) tracking
* Facilitate team/squad management across multiple athletes

### Data Management & Athlete Profile
* Create and manage athlete profiles with:
  * Unique UUID for each athlete (immutable identifier)
  * Name, gender (for event categorization), grade level, team/school
  * Editable profile information (can be updated at any time)
  * Optional notes/tags for coaching observations
* Support multiple athletes with separate seasonal records
* Track performance across full Ohio middle school track/field event season

### Meet/Event Registration & Recording
* Add/create track meet entries with:
  * Meet name and date
  * Location and meet type (invitational, conference, state, etc.)
  * Optional weather/conditions notes
* For each athlete at each meet:
  * Select events participated in (from Ohio track 2026 event list)
  * Record results for Track Events (times in MM:SS.MS format)
  * Record results for Field Events (distances in feet/inches or heights)
  * For relay events: track lane/heat assignment and individual leg splits (legs 1-4)
  * Optional: record finals qualification status, wind reading (for sprints), attempts/best (for field)

### Records/Results Area & Display
* Comprehensive records view with:
  * Display all meet results for all athletes (or filtered by athlete selection)
  * Sort by: meet date, event name, event number, result (time/distance), performance
  * Filter by:
    * Meet (single or multiple)
    * Athlete name (exact or fuzzy match)
    * Event (track or field, can select multiple)
    * Gender/Division
  * Search functionality: name, event, meet name using fuzzy matching
* Read mode (default): clean, organized display optimized for viewing/analysis
* Edit mode (toggle): enable inline editing of existing results with validation (think "edit vs. view" mode toggle)
* Delete capability: remove results or entire meet records
* Personal Record (PR) highlighting: visually flag best performances

### Data Analysis & Performance Tracking
* Display season statistics per athlete:
  * Best time/distance for each event
  * Improvement tracking (current vs. previous performance)
  * Number of attempts/participations per event
* Optional: graphical performance trends over season (simple charts/sparklines)
* Comparison view: compare athlete performance across same meet or same event

### Input/Entry Form Area
* Expandable/collapsible form for adding new meet records
* Form fields:
  * Meet selector (existing meets) or quick-add new meet (date selector)
  * Athlete selector (dropdown from existing athletes)
  * Event selector (filtered by gender, shows Ohio 2026 track/field events)
  * Result input (adaptive based on event type):
    * Time input (MM:SS.MS) for track events
    * Distance input (feet/inches) for long jump, discus, shot put
    * Height input (feet/inches) for high jump
  * Lane/Heat assignment (for relay events and applicable track events)
  * Relay leg number selector (for 4x events: legs 1, 2, 3, 4)
  * Optional fields: wind reading, attempt number, notes
* Form validation: prevent invalid time/distance entries, requires meet date and athlete
* Quick-add capability: add multiple results sequentially without re-filling meet/athlete

### Data Import/Export & Persistence
* Export all data to JSON format (download file)
* Import JSON data (merge or replace option)
* Auto-save to LocalStorage on every change
* Export as CSV for spreadsheet compatibility (optional)
* Data persistence survives browser closure and refresh

### User Interface & Accessibility
* Responsive layout: optimized for mobile (single column) and desktop (multi-column)
* Dark/Light mode toggle (optional but user-friendly)
* Clear visual hierarchy and intuitive navigation
* Accessible color contrasts and readable font sizes
* Touch-friendly buttons and inputs for mobile use
* Keyboard navigation support

### Out of Scope (Future Enhancements)
* Real-time meet updates during competition (to a cloud/3rd party site)
* User authentication or cloud sync
* Video replay integration
* Scheduling/heat assignment automation
* Team standings or ranking calculations


