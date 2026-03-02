## Design Rationale for Design system challenge - Arancia
In this fork from opensearh dashboard, I have implemented the token based design system that follows the standard approach to maintain scalability and consistency across the components. I have created ds_challenge_theme following softUI + Neumorphism design inspiration in which i have covered the following components to meet the requirements. 

1. Buttons
Introduced rounded borders, Branded styling, Hover impact, Accessible focus state, improved disabled behaviour.
2. Header
Improved background visibility, spacing for better experience, refined interaction experience, Typography improvements.
3. Sidebar Navigation
Alignment with custom generic theme, Improved active state with neumorphic styled impact, visual hierarchy improvements.
4. Cards
Neumorphic + soft radius and elevations, soft hover lift, spacing for the content, improved visual structure modern and fancy looks, Typography improvements.
5. Form Inputs
Shared input styling, Clear focus, consistent sizing and spacing, Fonts and Typography improvements.

## Custom Branding
Did custom branding as well with Arancia name and Logo to enhance the customization for branding.

## Additional User Experience Enhancements.
1. Global Search enhancement. Introduced recent search functionality to store recent search queries in LocalStorage for optimised and quick reusablity. Recent searches are stored in a limited scope inside the localstorage for quick access of recent searched item or query.

2. Implemented Search in sidebar for searching the Application like dashboard keeping in mind the complex hierarchy that bulks the sidebar with lots of recently viewed apps.
 
All changes are scoped to the specific relevent component. standards implementation of all changes no breaking of any of the state or functionality. 

# Setup and Build Instructions

## 1. Clone this Branch
Clone the repository and navigate into the project directory:

```bash
git clone -b design-system-challenge-task [https://github.com/imrbpro/DesignSystem-OpenSearch-Dashboard.git](https://github.com/imrbpro/DesignSystem-OpenSearch-Dashboard.git)
cd DesignSystem-OpenSearch-Dashboard
```

## 2. Install Yarn and Dependencies
OpenSearch Dashboards is set up using Yarn. To ensure you have the correct version, use corepack:
```bash
# Update corepack to the latest version
npm i -g corepack

# Install the correct version of yarn
corepack install

# Bootstrap the project dependencies
yarn osd bootstrap
```

### Run OpenSearch
OpenSearch Dashboards requires a running version of OpenSearch to connect to. You can choose to run OpenSearch locally yourself or point to an existing cluster.

### Run a local OpenSearch cluster
In a separate terminal, you can run the latest snapshot.

Note: This works for Linux, Windows, and macOS (Darwin). For other systems, use Docker or a tarball.

```bash
yarn opensearch snapshot
```

### Start OpenSearch Dashboards
Launch the development server:

```bash
yarn start
```

When the server is up and ready, the console will display:

```bash
[info][listening] Server running at http://localhost:5603/pgt
[info][server][OpenSearchDashboards][http] http server running at http://localhost:5603/pgt
```

Click on the link and dashboard will open on browser
