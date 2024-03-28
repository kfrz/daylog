# Personal Data Architecture Design

## Overview
The Personal Data Insights Project aims to leverage a diverse array of endogenous and exogenous data sources to generate meaningful insights into an individual's life, patterns, and experiences. By collecting, categorizing, and analyzing data from various aspects of an individual's digital footprint, this project seeks to create a comprehensive "quantified self" dashboard that provides personalized insights, recommendations, and reflections.
Based on the provided sources and your request for more precise, academic terminology to categorize the different types of data, here is a structured breakdown of the key terms and definitions:

## Data Categorization Taxonomy

### 1. Endogenous Data
- Definition: Data generated from within the system or entity being studied. This data arises as a direct result of the system's internal processes, interactions, and mechanics.
- Characteristics:
  - Intrinsic to the system
  - Emergent from the system's inherent properties and behaviors
  - Dependent on the system's internal logic and rules
- Examples:
  - In-game metrics (e.g., player scores, character attributes, virtual economy)
  - User-generated content within a platform (e.g., social media posts, forum discussions)
  - Transactional data from an organization's internal systems (e.g., sales records, employee performance metrics)

### 2. Exogenous Data
- Definition: Data originating from outside the system or entity being studied. This data represents external factors, influences, and conditions that impact the system but are not directly controlled by it.
- Characteristics:
  - Originates from the system's environment or context
  - Independent of the system's internal processes and mechanics
  - Affects the system's behavior and outcomes
- Examples:
  - Real-world weather data influencing in-game conditions
  - Economic indicators affecting a company's performance
  - Competitor actions impacting a firm's strategic decisions

### 3. Contextual Data
- Definition: Data that provides additional information about the context, setting, or circumstances surrounding the primary data being analyzed. This data helps to situate and interpret the main data points.
- Characteristics:
  - Supplements the primary data
  - Provides background information and context
  - Aids in understanding and interpreting the main data
- Examples:
  - Demographic data of game players
  - Industry benchmarks for comparing company performance
  - Historical data for trend analysis

### 4. Metadata
- Definition: Data that describes or provides information about other data. Metadata helps to organize, structure, and manage the primary data.
- Characteristics:
  - Descriptive information about data
  - Facilitates data discovery, understanding, and management
  - Enables efficient data organization and retrieval
- Examples:
  - Data dictionaries describing database fields and relationships
  - Tags and categories for content management systems
  - File properties (e.g., author, creation date, file type)

## Data Interaction Spectrum

### 1. Explicit Data Interaction
- Definition: Data that is directly and intentionally interacted with by the user or system. This data is actively manipulated, analyzed, or used to make decisions.
- Characteristics:
  - Consciously engaged with by the user or system
  - Directly influences actions and outcomes
  - Requires explicit input or manipulation
- Examples:
  - User input in forms and surveys
  - Querying a database for specific information
  - Adjusting game settings based on player preferences

### 2. Implicit Data Interaction
- Definition: Data that is indirectly or passively interacted with by the user or system. This data is not actively manipulated but still influences the system's behavior or user experience.
- Characteristics:
  - Not actively engaged with by the user or system
  - Indirectly affects the system's behavior or outcomes
  - Collected and used without explicit user input
- Examples:
  - User behavior tracking (e.g., click patterns, time spent on pages)
  - Recommender systems based on user preferences and history
  - Dynamic difficulty adjustment in games based on player performance

By using this structured taxonomy and spectrum, we can more precisely categorize and discuss the different types of data encountered in various systems and domains. This framework provides a common language and understanding for analyzing data interactions and their implications.


## Data Architecture
The project employs a robust data architecture that encompasses data collection, preprocessing, storage, and analysis. The architecture is designed to handle both structured and unstructured data from a wide range of sources, ensuring data integrity, security, and privacy throughout the pipeline.

### Key Components
1. Data Ingestion: Automated scripts and APIs are used to collect data from various sources, including internal generated data and external proxy data. The ingestion process ensures data quality and consistency.

2. Data Preprocessing: Raw data undergoes preprocessing to standardize formats, handle missing values, and extract relevant features. Techniques such as data normalization, feature scaling, and text processing are applied as needed.

3. Data Storage: Preprocessed data is stored in a centralized database optimized for efficient querying and analysis. The database schema is designed to accommodate the diverse data types and relationships present in the collected data.

4. Data Analysis: Advanced analytics techniques, including machine learning algorithms and natural language processing, are employed to derive insights from the data. The analysis focuses on pattern recognition, anomaly detection, and correlation discovery.

5. Insight Generation: The results of the data analysis are used to generate personalized insights, recommendations, and reflections. These insights are presented through an intuitive dashboard that allows users to explore their data and gain meaningful self-knowledge.

## Data Sources
The following is a comprehensive list of data sources utilized in the Personal Data Insights Project, categorized based on the data categorization taxonomy:

### Endogenous Data
1. Browser History (Explicit Data Interaction)
   - Websites visited
   - Time spent on each site
   - Bookmarks and saved pages
2. Git Commits (Explicit Data Interaction)
   - Code repositories
   - Commit messages and timestamps
   - Branch and merge history
3. Calendar Events (Explicit Data Interaction)
   - Scheduled meetings and appointments
   - Event durations and locations
   - Attendees and organizers
4. Email Data (Explicit Data Interaction)
   - Sent and received emails
   - Email metadata (timestamps, recipients, subject lines)
   - Email attachments and content
5. File System Data (Implicit Data Interaction)
   - File and folder structure
   - File metadata (creation dates, modifications, sizes)
   - Document content and types
6. Application Usage (Implicit Data Interaction)
   - Applications installed and used
   - Time spent in each application
   - Application-specific data and preferences
7. Social Media Data (Explicit Data Interaction)
   - Posts, tweets, and status updates
   - Social connections and interactions
   - Likes, comments, and shares
8. Biometric Data (Implicit Data Interaction)
   - Fitness tracker data (steps, heart rate, sleep patterns)
   - Smartwatch data (activity levels, stress levels)
   - Health app data (nutrition, medication, symptoms)

### Exogenous Data
1. Weather Data (Contextual Data)
   - Local weather conditions
   - Temperature, humidity, precipitation
   - Weather alerts and forecasts
2. News and World Events (Contextual Data)
   - News articles and headlines
   - Trending topics and hashtags
   - Global and local events
3. Financial Data (Contextual Data)
   - Stock prices and market trends
   - Economic indicators (GDP, inflation, unemployment rates)
   - Currency exchange rates
4. Geolocation Data (Implicit Data Interaction)
   - GPS coordinates and location history
   - Place visits and check-ins
   - Travel patterns and routes
5. Public Transportation Data (Contextual Data)
   - Bus and train schedules
   - Real-time transit updates
   - Traffic conditions and delays
6. Smart Home Data (Implicit Data Interaction)
   - Smart device usage (lights, thermostats, appliances)
   - Energy consumption and patterns
   - Home security and monitoring data
7. Environmental Data (Contextual Data)
   - Air quality and pollution levels
   - Pollen counts and allergen data
   - Noise levels and sound pollution

### Metadata
1. Data Dictionaries (Metadata)
   - Descriptions of data fields and attributes
   - Data types and constraints
   - Relationships between data entities
2. Data Lineage (Metadata)
   - Data source and origin information
   - Data transformation and processing history
   - Data version and update timestamps
3. Data Quality Metrics (Metadata)
   - Completeness and accuracy scores
   - Consistency and validity checks
   - Data freshness and timeliness indicators


By leveraging this extensive range of endogenous and exogenous data sources, along with the associated metadata, the Personal Data Insights Project aims to provide a holistic view of an individual's life and experiences. The project's data architecture and analysis capabilities enable the generation of meaningful insights that can help individuals better understand themselves, make informed decisions, and enhance their overall well-being.


Citations:
* [1] https://www.britannica.com/science/library-classification
* [2] https://digitalcommons.unl.edu/cgi/viewcontent.cgi?article=10205&context=libphilprac
* [3] https://www.questionpro.com/blog/categorical-data/
* [4] https://www.fullstory.com/blog/categorical-vs-quantitative-data/
* [5] https://csi.pressbooks.pub/lis/chapter/classification/
* [6] https://www.appinio.com/en/blog/market-research/categorical-data
* [7] https://en.wikipedia.org/wiki/Library_classification
* [8] https://csi.pressbooks.pub/lis/chapter/knowledge-information-and-data/
* [9] https://byjus.com/maths/categorical-data/
* [10] https://www.datacamp.com/blog/data-science-glossary
* [11] https://www.coursera.org/articles/data-science-terms
* [12] https://datacebo.com/blog/categorical-data/
* [13] https://data-planet.libguides.com/dataterminology
* [14] https://www.stat20.org/1-questions-and-data/02-taxonomy-of-data/notes
* [15] https://www.dataquest.io/blog/data-science-glossary/
* [16] https://academy.constructor.org/blog/data-science-terminology
* [17] https://www.reddit.com/r/truegaming/comments/dmygy3/internal_vs_external_logic_in_games/
* [18] https://www150.statcan.gc.ca/n1/edu/power-pouvoir/ch8/5214817-eng.htm
* [19] https://www.alteryx.com/glossary
