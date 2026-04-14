<p align="center">
<img width="642" height="205" alt="Screenshot 2026-04-14 174322" src="https://github.com/user-attachments/assets/38e82ca2-a879-4f6e-87e5-44d8b3afa32d" />
</p>
<h1><u>Milestone 8: HQ Wireless</u></h1>
    <p>Seventh phase, we will install 1 wireless access point for corporate network access via one SSID, and another wireless access point for guest network access via a different SSID.</p>
    <h2><strong><u>Configuration Steps</u></strong></h2>
    <p><b>Step 1: Install And Configure Corporate Wireless Access</b></p>
        <p>- A. Install An AccessPoint-PT And Connect It To HQ Core Switch 2 Into An Access Port</p>
        <p>- B. Configure The New AP With A Unique SSID, Channel, And Passphrase Using WPA2-PSK And AES</p>
        <p>- C. Install A Wireless Tablet And Configure It With The Same SSID And Passphrase</p>
        <p>- D. Once The New Wireless Tablet Is Connected Confirm It Has Access To The Corporate Networks And Internet</p>
    <p><b>Step 2: Install And Configure Guest Wireless Access</b></p>
        <p>- A. On The HQ Server Configure The DHCP Scope For The Guest Network</p>
            <p>- I. Default Gateway</p>
            <p>- II. DNS Server</p>
            <p>- III. Starting IP Address</p>
            <p>- IV. Subnet Mask</p>
            <p>- V. Number Of DHCP Users</p>
        <p>- B. On HQ Core Switches 1 And 2 Configure An Access-List That Only Allows DHCP And Internet Traffic For The Guest Network And Blocks All Other Traffic</p>
        <p>- C. On The HQ Core Switches 1 And 2 Apply The New Access-List To The VLAN 172 Interface</p>
        <p>- D. On The HQ Core Switch 1 And 2 Configure IP Helper In The VLAN 172 Interface</p>
        <p>- E. Configure A Switchport On HQ Access Switch 3 To Be A Member Of VLAN 172 (Guest)</p>
        <p>- F. Install A New AccessPoint-PT And Connect It To The Newly Configure Switchport On HQ Access Switch 3</p>
        <p>- G. Configure The New AP With A Unique SSID (GUEST), Channel, And Passphrase Using WPA2-PSK And AES</p>
        <p>- H. Install A Wireless Tablet And Configure It With The Same SSID And Passphrase</p>   
        <p>- I. Once The New Wireless Tablet Is Connected Confirm It Has Access To The Internet, But CANNOT Access Any Of The Corporate Networks.</p>
        <h2><strong><u>Implementation</u></strong></h2>
        <h3>Step 1: Install And Configure Corporate Wireless Access</h3>
            <p>- A. Install An AccessPoint-PT And Connect It To HQ Core Switch 2 Into An Access Port.</p>
            <p>- First, we will install a wireless access point to connect corporate wireless users to the data network.</p>
                <img width="939" height="884" alt="Screenshot 2026-04-14 181638" src="https://github.com/user-attachments/assets/ddb4e5c1-6c5b-40ee-a2c3-4494b93e067a" />\
            <p>- B. Configure The New AP With A Unique SSID, Channel, And Passphrase Using WPA2-PSK And AES</p>
                <img width="866" height="885" alt="Screenshot 2026-04-14 181922" src="https://github.com/user-attachments/assets/4d696d46-e485-46e1-a112-dbbe977ac824" />
            <p>- C. Install A Wireless Tablet And Configure It With The Same SSID And Passphrase</p>
                <img width="940" height="883" alt="Screenshot 2026-04-14 182154" src="https://github.com/user-attachments/assets/624c65b9-7f08-4157-98e6-6f0249f51f05" />
                <img width="867" height="882" alt="Screenshot 2026-04-14 182226" src="https://github.com/user-attachments/assets/b2acf45e-39ca-4fff-a4e0-bb92bfe43910" />
            <p>- D. Once The New Wireless Tablet Is Connected Confirm It Has Access To The Corporate Networks And Internet</p>
                <img width="871" height="1574" alt="Screenshot 2026-04-14 182528" src="https://github.com/user-attachments/assets/6da25638-1070-4782-bed2-610c6fb3fd56" />
                <img width="526" height="591" alt="Screenshot 2026-04-14 182621" src="https://github.com/user-attachments/assets/6a484e11-2c30-4624-b74c-2f0d957b64f5" />
            <p><em>- Successful.</em></p>
        <h3>Step 2: Install And Configure Guest Wireless Access</h3>
                <img width="868" height="256" alt="Screenshot 2026-04-14 165814" src="https://github.com/user-attachments/assets/b3126a7d-c1d7-479e-ae16-44efa5841035" />
        <h3>Step 3: On The HQ Voice Router Configure The Three Ephones That Were Just Connected</h3>
            <p>- Next, we'll access the HQ-VOICE-RTR CLI and configure the two new ephones.</p>
                <img width="872" height="881" alt="Screenshot 2026-04-14 165250" src="https://github.com/user-attachments/assets/46cac24e-109f-44b7-bb7f-febc5e03ec58" />
            <p><em>- After reloading the router, you can see that the uck9 licensing software was installed successfully.</em></p>
        <h3>Step 4: Test Dialing By Extension Between Each HQ Phone</h3>
            <p>- Next we will place calls between each phone by dialing the extensions from each phone.</p>
                <img width="1748" height="880" alt="Screenshot 2026-04-14 170113" src="https://github.com/user-attachments/assets/33df0337-9cc1-4668-be6a-786c0ab90553" />
                <img width="1739" height="881" alt="Screenshot 2026-04-14 170223" src="https://github.com/user-attachments/assets/f729314f-ac38-45f6-8c33-69096d9c8944" />
            <p><em>- We are successfully able to call between all 3 ephones.</em></p>
        <h3>Step 5: Test Outbound Dialing To The PSTN Test Phone 8885551111</h3>
                <img width="1750" height="879" alt="Screenshot 2026-04-14 170432" src="https://github.com/user-attachments/assets/8eee39c7-1495-4d7f-b29d-6378ab25e786" />
            <p><em>- Successful.</em></p>
       











            












 





