<h2>Automated IMDb Data Extraction Tool</h2>
<p>
    Developed an automated IMDb data extraction tool to retrieve movie and series details, including ratings, titles, and release dates. Enhanced the tool with error handling to efficiently manage missing or multiple results using UiPath.
</p>

<h3>Workflow Overview</h3>
<ul>
    <li>
        <strong>Google_Launch:</strong> Launching Google Chrome.<br>
        <em>PreCondition:</em> N/A<br>
        <em>PostCondition:</em> Search Bar Exists.
    </li>
    <li>
        <strong>Google_Search:</strong> Search Google Chrome.<br>
        <em>PreCondition:</em> Search Bar Exists.<br>
        <em>PostCondition:</em> All Buttons Exist.
    </li>
    <li>
        <strong>Google_First_Link:</strong> Click on First Link.<br>
        <em>PreCondition:</em> All Buttons Exist.<br>
        <em>PostCondition:</em> IMDb Search Bar Exists.
    </li>
    <li>
        <strong>IMDb_Search:</strong> Search in IMDb.<br>
        <em>PreCondition:</em> IMDb Search Bar Exists.<br>
        <em>PostCondition:</em> Search Exists.
    </li>
    <li>
        <strong>IMDb_Open_First_Title:</strong> Open and Click on the First Title Appeared.<br>
        <em>PreCondition:</em> Search Exists.<br>
        <em>PostCondition:</em> IMDb Data Container Exists.
    </li>
    <li>
        <strong>IMDb_Extracted_Data:</strong> Read and Extract the Search Prompt Data (Name, Rate, PG, Year, Duration).<br>
        <em>PreCondition:</em> IMDb Data Container Exists.<br>
        <em>PostCondition:</em> Data Extracted; IMDb Data Container Exists.
    </li>
    <li>
        <strong>Close_Tab:</strong> Close The Tab.<br>
        <em>PreCondition:</em> IMDb Logo Exists.<br>
        <em>PostCondition:</em> Tab Closed.
    </li>
    <li>
        <strong>Notepad_Write_List:</strong> Write Extracted Data to Notepad.<br>
        <em>PreCondition:</em> IMDb Data Exists.<br>
        <em>PostCondition:</em> Data Written to Notepad.
    </li>
</ul>
