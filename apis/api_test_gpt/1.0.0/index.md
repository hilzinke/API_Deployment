---
# NOTICE: Copyright 2024 Talend SA, Talend, Inc., and affiliates. All Rights Reserved. Customer’s use of the software contained herein is subject to the terms and conditions of the Agreement between Customer and Talend.
layout: "apiDefinition_1.1.0"
api-definition:
  specVersion: "4.1.0"
  info:
    name: "API_Test_GPT"
    version: "1.0.0"
    description: "Keine Beschreibung"
    license: {}
    contact: {}
  contract:
    baseUrls:
    - url: "http://localhost:8090"
      isPublished: true
    mediaTypes:
    - "application/json"
    unsortedElementOrder:
    - "#/contract/resources/987be9df-ccfc-44d4-b3b7-b54661baae45"
    - "#/contract/types/5f4862f9-a1ee-424e-bac7-6676e120628d"
    - "#/contract/resources/95bf7921-d4d9-4b77-a6a0-dcd6cd0cd53f"
    - "#/contract/resources/9bac2523-b1c1-418b-a091-53d39dc83a61"
    - "#/contract/resources/b1c98b33-a257-4d42-a730-b360370af756"
    - "#/contract/types/90705111-8346-4ed1-a84c-754ab2455336"
    - "#/contract/types/bde0b2f2-f2ed-46fd-82b4-1379b0d420c6"
    - "#/contract/types/ae8ef632-56f4-4930-ace5-b5ba1ad26274"
    - "#/contract/types/5f7a9686-d775-4a86-8651-db48a1d50f0a"
    - "#/contract/types/50ef1b31-92c7-4e6a-836e-423a8c15a20d"
    - "#/contract/types/920a4b32-aef4-4c73-8b8b-5b221f6f85c7"
    - "#/contract/types/2850be16-97e1-4266-bde2-d2e4b01b3909"
    - "#/contract/types/1acc6d93-458b-41ff-8bca-6eaf06ad5537"
    - "#/contract/types/d8857aaf-5b5b-4432-aecf-2f93f9338bd7"
    - "#/contract/types/745736da-a07b-432a-bdb2-4efeb0db4099"
    - "#/contract/types/dbed4348-4705-4022-afd1-183122036623"
    - "#/contract/types/2cfeee6f-a32c-40c5-a650-117722635a4b"
    - "#/contract/types/0b86c562-650b-49bc-a2b2-c13e5b5a7f0d"
    - "#/contract/types/157185b0-5fba-4c79-8115-8a852ade5ffe"
    - "#/contract/resources/f9dcf79f-a291-4f36-a750-975a3abf9c48"
    - "#/contract/resources/75c52026-e251-47b9-b105-3f67ea933a3e"
    - "#/contract/resources/e21399cb-de31-49ac-a7c4-b8d35d4165f9"
    - "#/contract/resources/e7f7b3c7-0bc8-42ba-8f0c-7d47d466d9b6"
    - "#/contract/resources/f466d634-216f-47d4-9791-07412af3af98"
    - "#/contract/resources/c0e5ecfb-e817-4c2a-92ce-a3c136468876"
    - "#/contract/types/96836d9b-0ec2-4a39-a20c-428b5d22710a"
    - "#/contract/resources/338b996b-e425-4dc0-9e2a-5b661ae265a8"
    - "#/contract/types/f3375145-7ef0-47bc-a467-63525dbba2ae"
    - "#/contract/resources/fb2a1f56-cec0-45eb-9190-46d01cf1af2e"
    - "#/contract/types/129b7ac3-0251-4721-83e9-b0a496885cf3"
    - "#/contract/resources/fe271c6b-0775-44d0-ad09-201954d7695a"
    resources:
      "987be9df-ccfc-44d4-b3b7-b54661baae45":
        name: "Fact entries of CDM"
        path: "/getFacts/{schema_hk}"
        pathVariables:
        - name: "schema_hk"
          type: "STRING"
          required: true
      "95bf7921-d4d9-4b77-a6a0-dcd6cd0cd53f":
        path: "/getFacts/"
        operations:
          "8f1c502a-9732-4039-95f3-9b505d54afdf":
            name: "/getFacts"
            method: "GET"
            operationId: "getFacts"
            queryParameters:
            - type: "#/components/queryParameters/ae8679cf-d0fc-454c-9ca3-a828fea3d6f1"
            - type: "#/components/queryParameters/4f57eb34-f444-4263-8348-f611aae1f553"
            responses:
              "90acd398-5274-47b6-a554-6a9e9c6b4647":
                status: "2XX"
                bodies:
                - type: "ARRAY"
                  items:
                    type: "#/contract/types/5f4862f9-a1ee-424e-bac7-6676e120628d"
                    required: false
                  examples:
                  - value: |-
                      <fact>
                      <row Schema_hk="b29015e368af9e66239f5ac48448b979" Schema="YCOA" Company_x0020_No="110" Company_hk="a87fdcf6948095213d6d2737659d64e7" Branch_x0020_No="1710" Date="2021-01-31T00:00:00" Date_hk="56acd4f269bafddc3987c14f4881bb54" Period="202101" Year="2021" Month="1" Account_hk="ada79b010949af6f7eb709d13110a81f" Account_x0020_No="10010000" Balance_x0020_Carried_x0020_Forward_x0020_Cn="Y" Balance_x0020_Carried_x0020_Forward="-9057.53" Monthly_x0020_begin_x0020_Balance="0.00" Monthly_x0020_Debit="0.00" Monthly_x0020_Credit="0.00" Monthly_x0020_Balance="-9057.53" Balance="-9057.53" Acceptance_x0020_Cn="N" Acceptance_x0020_Gr="10010000" Account_x0020_Monthly_x0020_Balance="-9057.53" Account_x0020_Balance="-9057.53" Gr_x0020_Monthly_x0020_Balance="-9057.53" Gr_x0020_Balance="-9057.53" Account_x0020_Type="Petty Cash" Account_x0020_Category="1" Account_x0020_Class="111100" Currency_x0020_Cc="USD" Currency_x0020_Gc="USD" Currency_x0020_Coc="CHF" Exchange_x0020_Rate_x0020_Cc_x0020_Gc="1.00000" Exchange_x0020_Rate_x0020_Gc_x0020_Coc="0.00000" Currency_x0020_Dim="1" rec_Load_ts="2023-04-12T09:30:26.730" rec_SourceSystem_str="SAP" />
                      <row Schema_hk="b29015e368af9e66239f5ac48448b979" Schema="YCOA" Company_x0020_No="110" Company_hk="a87fdcf6948095213d6d2737659d64e7" Branch_x0020_No="1710" Date="2021-01-31T00:00:00" Date_hk="56acd4f269bafddc3987c14f4881bb54" Period="202101" Year="2021" Month="1" Account_hk="ada79b010949af6f7eb709d13110a81f" Account_x0020_No="10010000" Balance_x0020_Carried_x0020_Forward_x0020_Cn="Y" Balance_x0020_Carried_x0020_Forward="-9157.53" Monthly_x0020_begin_x0020_Balance="-9057.53" Monthly_x0020_Debit="0.00" Monthly_x0020_Credit="0.00" Monthly_x0020_Balance="-100.00" Balance="-9157.53" Acceptance_x0020_Cn="N" Acceptance_x0020_Gr="10010000" Account_x0020_Monthly_x0020_Balance="-100.00" Account_x0020_Balance="-9157.53" Gr_x0020_Monthly_x0020_Balance="-100.00" Gr_x0020_Balance="-9157.53" Account_x0020_Type="Petty Cash" Account_x0020_Category="1" Account_x0020_Class="111100" Currency_x0020_Cc="USD" Currency_x0020_Gc="USD" Currency_x0020_Coc="CHF" Exchange_x0020_Rate_x0020_Cc_x0020_Gc="1.00000" Exchange_x0020_Rate_x0020_Gc_x0020_Coc="0.00000" Currency_x0020_Dim="1" rec_Load_ts="2023-04-12T09:30:26.750" rec_SourceSystem_str="SAP" />
                      <row Schema_hk="b29015e368af9e66239f5ac48448b979" Schema="YCOA" Company_x0020_No="110" Company_hk="a87fdcf6948095213d6d2737659d64e7" Branch_x0020_No="1710" Date="2021-01-31T00:00:00" Date_hk="56acd4f269bafddc3987c14f4881bb54" Period="202101" Year="2021" Month="1" Account_hk="ada79b010949af6f7eb709d13110a81f" Account_x0020_No="10010000" Balance_x0020_Carried_x0020_Forward_x0020_Cn="Y" Balance_x0020_Carried_x0020_Forward="-5560.71" Monthly_x0020_begin_x0020_Balance="-9157.53" Monthly_x0020_Debit="0.00" Monthly_x0020_Credit="0.00" Monthly_x0020_Balance="3596.82" Balance="-5560.71" Acceptance_x0020_Cn="N" Acceptance_x0020_Gr="10010000" Account_x0020_Monthly_x0020_Balance="3596.82" Account_x0020_Balance="-5560.71" Gr_x0020_Monthly_x0020_Balance="3596.82" Gr_x0020_Balance="-5560.71" Account_x0020_Type="Petty Cash" Account_x0020_Category="1" Account_x0020_Class="111100" Currency_x0020_Cc="USD" Currency_x0020_Gc="USD" Currency_x0020_Coc="CHF" Exchange_x0020_Rate_x0020_Cc_x0020_Gc="1.00000" Exchange_x0020_Rate_x0020_Gc_x0020_Coc="0.00000" Currency_x0020_Dim="1" rec_Load_ts="2023-04-12T09:30:26.757" rec_SourceSystem_str="SAP" />
                      <row Schema_hk="b29015e368af9e66239f5ac48448b979" Schema="YCOA" Company_x0020_No="110" Company_hk="a87fdcf6948095213d6d2737659d64e7" Branch_x0020_No="1710" Date="2021-01-31T00:00:00" Date_hk="56acd4f269bafddc3987c14f4881bb54" Period="202101" Year="2021" Month="1" Account_hk="ada79b010949af6f7eb709d13110a81f" Account_x0020_No="10010000" Balance_x0020_Carried_x0020_Forward_x0020_Cn="N" Balance_x0020_Carried_x0020_Forward="-5560.71" Monthly_x0020_begin_x0020_Balance="-5560.71" Monthly_x0020_Debit="0.00" Monthly_x0020_Credit="0.00" Monthly_x0020_Balance="0.00" Balance="-5560.71" Acceptance_x0020_Cn="N" Acceptance_x0020_Gr="10010000" Account_x0020_Monthly_x0020_Balance="0.00" Account_x0020_Balance="-5560.71" Gr_x0020_Monthly_x0020_Balance="0.00" Gr_x0020_Balance="-5560.71" Account_x0020_Type="Petty Cash" Account_x0020_Category="1" Account_x0020_Class="111100" Currency_x0020_Cc="USD" Currency_x0020_Gc="USD" Currency_x0020_Coc="CHF" Exchange_x0020_Rate_x0020_Cc_x0020_Gc="1.00000" Exchange_x0020_Rate_x0020_Gc_x0020_Coc="0.00000" Currency_x0020_Dim="1" rec_Load_ts="2023-04-12T09:30:26.760" rec_SourceSystem_str="SAP" />
                      <row Schema_hk="b29015e368af9e66239f5ac48448b979" Schema="YCOA" Company_x0020_No="110" Company_hk="a87fdcf6948095213d6d2737659d64e7" Branch_x0020_No="1710" Date="2021-01-31T00:00:00" Date_hk="56acd4f269bafddc3987c14f4881bb54" Period="202101" Year="2021" Month="1" Account_hk="ada79b010949af6f7eb709d13110a81f" Account_x0020_No="10010000" Balance_x0020_Carried_x0020_Forward_x0020_Cn="N" Balance_x0020_Carried_x0020_Forward="-5560.71" Monthly_x0020_begin_x0020_Balance="-5560.71" Monthly_x0020_Debit="9200.00" Monthly_x0020_Credit="-5000.00" Monthly_x0020_Balance="4200.00" Balance="-1360.71" Acceptance_x0020_Cn="N" Acceptance_x0020_Gr="10010000" Account_x0020_Monthly_x0020_Balance="4200.00" Account_x0020_Balance="-1360.71" Gr_x0020_Monthly_x0020_Balance="4200.00" Gr_x0020_Balance="-1360.71" Account_x0020_Type="Petty Cash" Account_x0020_Category="1" Account_x0020_Class="111100" Currency_x0020_Cc="USD" Currency_x0020_Gc="USD" Currency_x0020_Coc="CHF" Exchange_x0020_Rate_x0020_Cc_x0020_Gc="1.00000" Exchange_x0020_Rate_x0020_Gc_x0020_Coc="0.00000" Currency_x0020_Dim="1" rec_Load_ts="2023-04-12T09:30:26.763" rec_SourceSystem_str="SAP" />
                      <row Schema_hk="b29015e368af9e66239f5ac48448b979" Schema="YCOA" Company_x0020_No="110" Company_hk="a87fdcf6948095213d6d2737659d64e7" Branch_x0020_No="1710" Date="2021-01-31T00:00:00" Date_hk="56acd4f269bafddc3987c14f4881bb54" Period="202101" Year="2021" Month="1" Account_hk="ada79b010949af6f7eb709d13110a81f" Account_x0020_No="10010000" Balance_x0020_Carried_x0020_Forward_x0020_Cn="N" Balance_x0020_Carried_x0020_Forward="-5560.71" Monthly_x0020_begin_x0020_Balance="-1360.71" Monthly_x0020_Debit="0.00" Monthly_x0020_Credit="0.00" Monthly_x0020_Balance="0.00" Balance="-1360.71" Acceptance_x0020_Cn="N" Acceptance_x0020_Gr="10010000" Account_x0020_Monthly_x0020_Balance="0.00" Account_x0020_Balance="-1360.71" Gr_x0020_Monthly_x0020_Balance="0.00" Gr_x0020_Balance="-1360.71" Account_x0020_Type="Petty Cash" Account_x0020_Category="1" Account_x0020_Class="111100" Currency_x0020_Cc="USD" Currency_x0020_Gc="USD" Currency_x0020_Coc="CHF" Exchange_x0020_Rate_x0020_Cc_x0020_Gc="1.00000" Exchange_x0020_Rate_x0020_Gc_x0020_Coc="0.00000" Currency_x0020_Dim="1" rec_Load_ts="2023-04-12T09:30:26.770" rec_SourceSystem_str="SAP" />
                      <row Schema_hk="b29015e368af9e66239f5ac48448b979" Schema="YCOA" Company_x0020_No="110" Company_hk="a87fdcf6948095213d6d2737659d64e7" Branch_x0020_No="1710" Date="2021-02-28T00:00:00" Date_hk="a1ccae0dceda99f0fb938b374d34e723" Period="202102" Year="2021" Month="2" Account_hk="ada79b010949af6f7eb709d13110a81f" Account_x0020_No="10010000" Balance_x0020_Carried_x0020_Forward_x0020_Cn="N" Balance_x0020_Carried_x0020_Forward="-5560.71" Monthly_x0020_begin_x0020_Balance="-1360.71" Monthly_x0020_Debit="0.00" Monthly_x0020_Credit="0.00" Monthly_x0020_Balance="0.00" Balance="-1360.71" Acceptance_x0020_Cn="N" Acceptance_x0020_Gr="10010000" Account_x0020_Monthly_x0020_Balance="0.00" Account_x0020_Balance="-1360.71" Gr_x0020_Monthly_x0020_Balance="0.00" Gr_x0020_Balance="-1360.71" Account_x0020_Type="Petty Cash" Account_x0020_Category="1" Account_x0020_Class="111100" Currency_x0020_Cc="USD" Currency_x0020_Gc="USD" Currency_x0020_Coc="CHF" Exchange_x0020_Rate_x0020_Cc_x0020_Gc="1.00000" Exchange_x0020_Rate_x0020_Gc_x0020_Coc="0.00000" Currency_x0020_Dim="1" rec_Load_ts="2023-04-12T09:30:26.770" rec_SourceSystem_str="SAP" />
                      <row Schema_hk="b29015e368af9e66239f5ac48448b979" Schema="YCOA" Company_x0020_No="110" Company_hk="a87fdcf6948095213d6d2737659d64e7" Branch_x0020_No="1710" Date="2021-02-28T00:00:00" Date_hk="a1ccae0dceda99f0fb938b374d34e723" Period="202102" Year="2021" Month="2" Account_hk="ada79b010949af6f7eb709d13110a81f" Account_x0020_No="10010000" Balance_x0020_Carried_x0020_Forward_x0020_Cn="N" Balance_x0020_Carried_x0020_Forward="-5560.71" Monthly_x0020_begin_x0020_Balance="-1360.71" Monthly_x0020_Debit="0.00" Monthly_x0020_Credit="0.00" Monthly_x0020_Balance="0.00" Balance="-1360.71" Acceptance_x0020_Cn="N" Acceptance_x0020_Gr="10010000" Account_x0020_Monthly_x0020_Balance="0.00" Account_x0020_Balance="-1360.71" Gr_x0020_Monthly_x0020_Balance="0.00" Gr_x0020_Balance="-1360.71" Account_x0020_Type="Petty Cash" Account_x0020_Category="1" Account_x0020_Class="111100" Currency_x0020_Cc="USD" Currency_x0020_Gc="USD" Currency_x0020_Coc="CHF" Exchange_x0020_Rate_x0020_Cc_x0020_Gc="1.00000" Exchange_x0020_Rate_x0020_Gc_x0020_Coc="0.00000" Currency_x0020_Dim="1" rec_Load_ts="2023-04-12T09:30:26.773" rec_SourceSystem_str="SAP" />
                      <row Schema_hk="b29015e368af9e66239f5ac48448b979" Schema="YCOA" Company_x0020_No="110" Company_hk="a87fdcf6948095213d6d2737659d64e7" Branch_x0020_No="1710" Date="2021-02-28T00:00:00" Date_hk="a1ccae0dceda99f0fb938b374d34e723" Period="202102" Year="2021" Month="2" Account_hk="ada79b010949af6f7eb709d13110a81f" Account_x0020_No="10010000" Balance_x0020_Carried_x0020_Forward_x0020_Cn="N" Balance_x0020_Carried_x0020_Forward="-5560.71" Monthly_x0020_begin_x0020_Balance="-1360.71" Monthly_x0020_Debit="0.00" Monthly_x0020_Credit="0.00" Monthly_x0020_Balance="0.00" Balance="-1360.71" Acceptance_x0020_Cn="N" Acceptance_x0020_Gr="10010000" Account_x0020_Monthly_x0020_Balance="0.00" Account_x0020_Balance="-1360.71" Gr_x0020_Monthly_x0020_Balance="0.00" Gr_x0020_Balance="-1360.71" Account_x0020_Type="Petty Cash" Account_x0020_Category="1" Account_x0020_Class="111100" Currency_x0020_Cc="USD" Currency_x0020_Gc="USD" Currency_x0020_Coc="CHF" Exchange_x0020_Rate_x0020_Cc_x0020_Gc="1.00000" Exchange_x0020_Rate_x0020_Gc_x0020_Coc="0.00000" Currency_x0020_Dim="1" rec_Load_ts="2023-04-12T09:30:26.777" rec_SourceSystem_str="SAP" />
                      <row Schema_hk="b29015e368af9e66239f5ac48448b979" Schema="YCOA" Company_x0020_No="110" Company_hk="a87fdcf6948095213d6d2737659d64e7" Branch_x0020_No="1710" Date="2021-03-31T00:00:00" Date_hk="94dbf171ceac4ce3106b93f3ad4d41a4" Period="202103" Year="2021" Month="3" Account_hk="ada79b010949af6f7eb709d13110a81f" Account_x0020_No="10010000" Balance_x0020_Carried_x0020_Forward_x0020_Cn="N" Balance_x0020_Carried_x0020_Forward="-5560.71" Monthly_x0020_begin_x0020_Balance="-1360.71" Monthly_x0020_Debit="0.00" Monthly_x0020_Credit="0.00" Monthly_x0020_Balance="0.00" Balance="-1360.71" Acceptance_x0020_Cn="N" Acceptance_x0020_Gr="10010000" Account_x0020_Monthly_x0020_Balance="0.00" Account_x0020_Balance="-1360.71" Gr_x0020_Monthly_x0020_Balance="0.00" Gr_x0020_Balance="-1360.71" Account_x0020_Type="Petty Cash" Account_x0020_Category="1" Account_x0020_Class="111100" Currency_x0020_Cc="USD" Currency_x0020_Gc="USD" Currency_x0020_Coc="CHF" Exchange_x0020_Rate_x0020_Cc_x0020_Gc="1.00000" Exchange_x0020_Rate_x0020_Gc_x0020_Coc="0.00000" Currency_x0020_Dim="1" rec_Load_ts="2023-04-12T09:30:26.780" rec_SourceSystem_str="SAP" />
                      </fact>
      "9bac2523-b1c1-418b-a091-53d39dc83a61":
        path: "/getDimensions/"
      b1c98b33-a257-4d42-a730-b360370af756:
        path: "/getDimensions/Accounts"
        operations:
          "54c5c001-9844-4c82-b89d-338578f5860d":
            name: "getAccounts"
            method: "GET"
            queryParameters:
            - type: "#/components/queryParameters/ae8679cf-d0fc-454c-9ca3-a828fea3d6f1"
            - type: "#/components/queryParameters/4f57eb34-f444-4263-8348-f611aae1f553"
            responses:
              df8d3a33-deba-402f-8b44-ade862cbf7cb:
                status: "2XX"
                bodies:
                - type: "ARRAY"
                  items:
                    type: "#/contract/types/bde0b2f2-f2ed-46fd-82b4-1379b0d420c6"
                    required: false
                  mediaTypes:
                  - "application/xml"
      f9dcf79f-a291-4f36-a750-975a3abf9c48:
        path: "/getDimensions/Calendars"
        operations:
          "0e945b02-2797-400a-be22-6467e8cf11bf":
            name: "getCalendars"
            method: "GET"
            queryParameters:
            - type: "#/components/queryParameters/ae8679cf-d0fc-454c-9ca3-a828fea3d6f1"
            - type: "#/components/queryParameters/4f57eb34-f444-4263-8348-f611aae1f553"
            responses:
              d962f7b4-badb-41da-9882-af25cb843801:
                status: "2XX"
                bodies:
                - type: "ARRAY"
                  items:
                    type: "#/contract/types/5f7a9686-d775-4a86-8651-db48a1d50f0a"
                    required: false
                  examples:
                  - value: |-
                      <calendars>
                        <row Calendar_hk="000eff92bb9e1969710c72c5bac2de03" Date="2021-01-02T00:00:00" Date_int="20210102" Week="1" Year="2021" Month_num="1" Day="2" Quarter_num="1" HalfYear_num="1" Weekday_num="6" Weekday="Saturday" Month="January" Quarter="1. Quarter" Half_x0020_Year="1. HalfYear" Workday="0" rec_Load_ts="2023-06-07T10:20:56.823" rec_SourceSystem_str="CORE" />
                        <row Calendar_hk="000eff92bb9e1969710c72c5bac2de03" Date="2021-01-02T00:00:00" Date_int="20210102" Week="1" Year="2021" Month_num="1" Day="2" Quarter_num="1" HalfYear_num="1" Weekday_num="6" Weekday="Saturday" Month="January" Quarter="1. Quarter" Half_x0020_Year="1. HalfYear" Workday="0" rec_Load_ts="2023-06-07T10:20:56.823" rec_SourceSystem_str="CORE" />
                      </calendars>
                  mediaTypes:
                  - "application/xml"
      "75c52026-e251-47b9-b105-3f67ea933a3e":
        path: "/getDimensions/Costcenters"
        operations:
          "1e4fad66-00b9-4da9-9201-0840fa0a8315":
            name: "getCostcenters"
            method: "GET"
            queryParameters:
            - type: "#/components/queryParameters/ae8679cf-d0fc-454c-9ca3-a828fea3d6f1"
            - type: "#/components/queryParameters/4f57eb34-f444-4263-8348-f611aae1f553"
            responses:
              "57d72567-202c-4a24-8acc-d7cf34399b1c":
                status: "2XX"
                bodies:
                - type: "ARRAY"
                  items:
                    type: "#/contract/types/920a4b32-aef4-4c73-8b8b-5b221f6f85c7"
                    required: false
                  examples:
                  - value: |-
                      <costcenters>
                        <row CostCentreHK="c4ca4238a0b923820dcc509a6f75849b" CostCentreID="1" CostCentre="Austria" />
                        <row CostCentreHK="c4ca4238a0b923820dcc509a6f75849b" CostCentreID="1" CostCentre="Austria" />
                        <row CostCentreHK="c4ca4238a0b923820dcc509a6f75849b" CostCentreID="1" CostCentre="Austria" />
                      </costcenters>
                  mediaTypes:
                  - "application/xml"
      e21399cb-de31-49ac-a7c4-b8d35d4165f9:
        path: "/getDimensions/Departments"
        operations:
          cfa2c36b-f716-4ced-a296-58991adae5f5:
            name: "getDepartments"
            method: "GET"
            queryParameters:
            - type: "#/components/queryParameters/ae8679cf-d0fc-454c-9ca3-a828fea3d6f1"
            - type: "#/components/queryParameters/4f57eb34-f444-4263-8348-f611aae1f553"
            responses:
              "357eeb23-48c0-4489-a183-32aced0faaf8":
                status: "2XX"
                bodies:
                - type: "ARRAY"
                  items:
                    type: "#/contract/types/1acc6d93-458b-41ff-8bca-6eaf06ad5537"
                    required: false
                  examples:
                  - value: |-
                      <departments>
                        <row DepartmentHK="a87ff679a2f3e71d9181a67b7542122c" DepartmentID="4" Department="Operations" />
                        <row DepartmentHK="a87ff679a2f3e71d9181a67b7542122c" DepartmentID="4" Department="Operations" />
                      </departments>
                  mediaTypes:
                  - "application/xml"
      e7f7b3c7-0bc8-42ba-8f0c-7d47d466d9b6:
        path: "/getDimensions/Employees"
        operations:
          "4e71284d-961e-46bd-b401-4129a76a58ef":
            name: "getEmployees"
            method: "GET"
            queryParameters:
            - type: "#/components/queryParameters/ae8679cf-d0fc-454c-9ca3-a828fea3d6f1"
            - type: "#/components/queryParameters/4f57eb34-f444-4263-8348-f611aae1f553"
            responses:
              c5a18c61-1972-4dfc-8142-306a3c474bbf:
                status: "2XX"
                bodies:
                - type: "ARRAY"
                  items:
                    type: "#/contract/types/745736da-a07b-432a-bdb2-4efeb0db4099"
                    required: false
                  examples:
                  - value: |-
                      <employees>
                        <row EmployeeSK="9060" EmployeeHK="20c097b913a26ba121cd74da10e7558f" EmployeeNumber="BC7249" EntryDate="2023-02-01T00:00:00" CompanyRegNo="HICO.00002" CompanyName="HICO Demo " FirstNames="Baby" Surname="Thibela" CurrentEmployeeStatus="Active" MaritalStatus="Single / Never Married" EmployeeStatus="Active" CurrentStatusEffectiveDate="26/02/2023" Race="Coloured" Gender="Male" Nationality="ZAF" ForeignNational="National" DateOfBirth="1970-06-05T00:00:00" JobGrade="Entry-level" JobGradeHK="c4ca4238a0b923820dcc509a6f75849b" JobGradeEffectiveDate="26/02/2023" JobTitle="Clerk" JobTitleEffectiveDate="26/02/2023" OccupationalLevel="Unskilled &amp; Defined Decision Makers" OccupationalCatagory="Service and Sales Workers" CostCentre="Germany" CostCentreHK="c81e728d9d4c2f636f067f89cc14862c" CostCentreEffectiveDate="26/02/2023" Department="Marketing &amp; Sales" DepartmentHK="c81e728d9d4c2f636f067f89cc14862c" DepartmentEffectiveDate="26/02/2023" EmploymentType="Temporary" ExitDate="9999-12-31T00:00:00" ContractDate="2023-02-26T00:00:00" ExitDateHK="2f4e01157c1afb7db9137fbc27dc9f09" ContractDateHK="4a153d17df87bc956ba907b15e68b7cb" IntervalFromDate="2023-02-01T00:00:00" Hashdiff="3d6a5cae11570d5bc416e5e46cfe35aa" scd_start="2023-02-26T00:00:00" scd_version="2" scd_active="1" />
                        <row EmployeeSK="9060" EmployeeHK="20c097b913a26ba121cd74da10e7558f" EmployeeNumber="BC7249" EntryDate="2023-02-01T00:00:00" CompanyRegNo="HICO.00002" CompanyName="HICO Demo " FirstNames="Baby" Surname="Thibela" CurrentEmployeeStatus="Active" MaritalStatus="Single / Never Married" EmployeeStatus="Active" CurrentStatusEffectiveDate="26/02/2023" Race="Coloured" Gender="Male" Nationality="ZAF" ForeignNational="National" DateOfBirth="1970-06-05T00:00:00" JobGrade="Entry-level" JobGradeHK="c4ca4238a0b923820dcc509a6f75849b" JobGradeEffectiveDate="26/02/2023" JobTitle="Clerk" JobTitleEffectiveDate="26/02/2023" OccupationalLevel="Unskilled &amp; Defined Decision Makers" OccupationalCatagory="Service and Sales Workers" CostCentre="Germany" CostCentreHK="c81e728d9d4c2f636f067f89cc14862c" CostCentreEffectiveDate="26/02/2023" Department="Marketing &amp; Sales" DepartmentHK="c81e728d9d4c2f636f067f89cc14862c" DepartmentEffectiveDate="26/02/2023" EmploymentType="Temporary" ExitDate="9999-12-31T00:00:00" ContractDate="2023-02-26T00:00:00" ExitDateHK="2f4e01157c1afb7db9137fbc27dc9f09" ContractDateHK="4a153d17df87bc956ba907b15e68b7cb" IntervalFromDate="2023-02-01T00:00:00" Hashdiff="3d6a5cae11570d5bc416e5e46cfe35aa" scd_start="2023-02-26T00:00:00" scd_version="2" scd_active="1" />
                      </employees>
                  mediaTypes:
                  - "application/xml"
      f466d634-216f-47d4-9791-07412af3af98:
        path: "/getDimensions/Grades"
        operations:
          da593950-f72b-42dc-b714-7aaaa6f24efc:
            name: "getGrades"
            method: "GET"
            queryParameters:
            - type: "#/components/queryParameters/ae8679cf-d0fc-454c-9ca3-a828fea3d6f1"
            - type: "#/components/queryParameters/4f57eb34-f444-4263-8348-f611aae1f553"
            responses:
              c5d947d3-9793-4c47-b64e-f8c1e9e58b87:
                status: "2XX"
                bodies:
                - type: "ARRAY"
                  items:
                    type: "#/contract/types/2cfeee6f-a32c-40c5-a650-117722635a4b"
                    required: false
                  examples:
                  - value: |-
                      <grades>
                        <row JobGradeHK="1679091c5a880faf6fb5e6087eb1b2dc" JobGradeID="6" JobGrade="Senior Management" />
                        <row JobGradeHK="1679091c5a880faf6fb5e6087eb1b2dc" JobGradeID="6" JobGrade="Senior Management" />
                      </grades>
                  mediaTypes:
                  - "application/xml"
      c0e5ecfb-e817-4c2a-92ce-a3c136468876:
        path: "/getDimensions/Salaries"
        operations:
          "36eb9a25-afbd-460a-bf0b-0cbf9f686bbb":
            name: "getSalary"
            method: "GET"
            queryParameters:
            - type: "#/components/queryParameters/ae8679cf-d0fc-454c-9ca3-a828fea3d6f1"
            - type: "#/components/queryParameters/4f57eb34-f444-4263-8348-f611aae1f553"
            responses:
              "6ed2f93e-3d60-4c94-b2d5-978ef29c1048":
                status: "200"
                bodies:
                - type: "ARRAY"
                  items:
                    type: "#/contract/types/157185b0-5fba-4c79-8115-8a852ade5ffe"
                    required: false
                  examples:
                  - value: |-
                      <salaries>
                        <row EmployeeSK="1018" EmployeeHK="55507ef387f98cdb7edafe7fa0bdd77f" EmployeeNumber="BC2649" IntervalFromDateHK="9630953f8423d4587a7b88896f72598f" IntervalFromDate="2020-10-01T00:00:00" IntervalToDateHK="a712bd324387f05f8e63ed6462cc3f0b" IntervalToDate="2020-10-31T00:00:00" TaxYear="2021" CompanyRegNo="HICO.00002" NormalCashPay="3090.00" TotalPackageValue="3090.00" TotalGrossCashPay="3090.00" TotalNettPay="3059.10" TotalCostToCompany="3090.00" TotalOvertimeHours="0.00" TotalOvertimeValue="0.00" TotalNormalTimeHours="173.36" TotalNormalTimeValue="3090.00" TotalBonuses="0.00" TotalGroupIncome="3090.00" TotalGroupOccasional="0.00" TotalGroupDeductions="30.90" TotalGroupStatutory="30.90" TotalEmployeesTax="0.00" TotalTaxAbatements="-30.90" TotalUIF="61.80" TotalSDL="30.90" UIFRemuneration="3090.00" SDLRemuneration="3090.00" OIDARemuneration="3090.00" />
                        <row EmployeeSK="1018" EmployeeHK="55507ef387f98cdb7edafe7fa0bdd77f" EmployeeNumber="BC2649" IntervalFromDateHK="9630953f8423d4587a7b88896f72598f" IntervalFromDate="2020-10-01T00:00:00" IntervalToDateHK="a712bd324387f05f8e63ed6462cc3f0b" IntervalToDate="2020-10-31T00:00:00" TaxYear="2021" CompanyRegNo="HICO.00002" NormalCashPay="3090.00" TotalPackageValue="3090.00" TotalGrossCashPay="3090.00" TotalNettPay="3059.10" TotalCostToCompany="3090.00" TotalOvertimeHours="0.00" TotalOvertimeValue="0.00" TotalNormalTimeHours="173.36" TotalNormalTimeValue="3090.00" TotalBonuses="0.00" TotalGroupIncome="3090.00" TotalGroupOccasional="0.00" TotalGroupDeductions="30.90" TotalGroupStatutory="30.90" TotalEmployeesTax="0.00" TotalTaxAbatements="-30.90" TotalUIF="61.80" TotalSDL="30.90" UIFRemuneration="3090.00" SDLRemuneration="3090.00" OIDARemuneration="3090.00" />
                        </salaries>
                  mediaTypes:
                  - "application/xml"
      "338b996b-e425-4dc0-9e2a-5b661ae265a8":
        path: "/getFacts/Balance"
        operations:
          dde1f81d-7738-45b1-81f1-a8d54b3b971d:
            name: "getBalance"
            method: "GET"
            queryParameters:
            - type: "#/components/queryParameters/ae8679cf-d0fc-454c-9ca3-a828fea3d6f1"
            - type: "#/components/queryParameters/4f57eb34-f444-4263-8348-f611aae1f553"
            responses:
              "8154777e-71b7-4485-bcfa-68d251346321":
                status: "2XX"
                bodies:
                - type: "ARRAY"
                  items:
                    type: "#/contract/types/f3375145-7ef0-47bc-a467-63525dbba2ae"
                    required: false
                  examples:
                  - value: "<fact><row Schema_hk=\"9d8b572681dd1c0798df20cbf08fd662\" Schema=\"YCOA\" Company_hk=\"a87fdcf6948095213d6d2737659d64e7\" Date_hk=\"56acd4f269bafddc3987c14f4881bb54\" Period=\"202101\" Balance_x0020_Carried_x0020_Forward_x0020_Cn=\"Y\" Balance_x0020_Carried_x0020_Forward=\"-35119.96\" Monthly_x0020_begin_x0020_Balance=\"0.00\" Monthly_x0020_Debit=\"0.00\" Monthly_x0020_Credit=\"0.00\" Monthly_x0020_Balance=\"-35119.96\" Balance=\"-35119.96\" Account_x0020_Monthly_x0020_Balance=\"0.00\" Account_x0020_Balance=\"0.00\" Gr_x0020_Monthly_x0020_Balance=\"0.00\" Gr_x0020_Balance=\"0.00\" Currency_x0020_Cc=\"USD\" Currency_x0020_Gc=\"USD\" Currency_x0020_Coc=\"CHF\" Exchange_x0020_Rate_x0020_Cc_x0020_Gc=\"1.00000\" Exchange_x0020_Rate_x0020_Gc_x0020_Coc=\"0.00000\" Currency_x0020_Dim=\"1\" Calendar_hk=\"56acd4f269bafddc3987c14f4881bb54\" Date_int=\"20210131\" Week=\"6\" Month_num=\"1\" Day=\"31\" Quarter_num=\"1\" HalfYear_num=\"1\" Weekday_num=\"7\" Weekday=\"Sunday\" Quarter=\"1. Quarter\" Half_x0020_Year=\"1. HalfYear\" Account_hk=\"0\" Company_x0020_Area_x0020_No=\"1000\" Account_x0020_Plan=\"YCOA\" Consolid_x0020_Account_x0020_No=\"111100\" Account_id=\"110_1710_YCOA_11001000\" Account_x0020_Text=\"Bank 1 - Bank (Main) Account\" Account_x0020_Class_x0020_Text=\"B_BILANZ\" Liquidity_x0020_Cn=\"N\" Overdraft=\"0.00\" Creation_x0020_Year=\"2\" /></fact>"
      fb2a1f56-cec0-45eb-9190-46d01cf1af2e:
        path: "/getFacts/Employee"
        operations:
          a42ca501-608d-4687-a306-43ddf6b9e0c8:
            name: "getEmployeeSPOT"
            method: "GET"
            queryParameters:
            - type: "#/components/queryParameters/ae8679cf-d0fc-454c-9ca3-a828fea3d6f1"
            - type: "#/components/queryParameters/4f57eb34-f444-4263-8348-f611aae1f553"
            responses:
              "8bb84232-1dd6-4ba1-8dd6-e86ca75d61cf":
                status: "2XX"
                bodies:
                - type: "ARRAY"
                  items:
                    type: "#/contract/types/129b7ac3-0251-4721-83e9-b0a496885cf3"
                    required: false
                  examples:
                  - value: "<row EntryDate=\"2020-03-01T00:00:00\" CompanyName=\"HICO Demo \" FirstNames=\"Magomarele\" Surname=\"Shetunyenga\" CurrentEmployeeStatus=\"Active\" MaritalStatus=\"Widowed\" EmployeeStatus=\"Active\" CurrentStatusEffectiveDate=\"27/03/2019\" Race=\"Other\" Gender=\"Female\" Nationality=\"ZAF\" ForeignNational=\"National\" DateOfBirth=\"1968-12-31T00:00:00\" JobGradeEffectiveDate=\"27/03/2019\" JobTitle=\"Data Entry Clerk\" JobTitleEffectiveDate=\"27/03/2019\" OccupationalLevel=\"Unskilled &amp; Defined Decision Makers\" OccupationalCatagory=\"Service and Sales Workers\" CostCentreEffectiveDate=\"27/03/2019\" DepartmentEffectiveDate=\"27/03/2019\" EmploymentType=\"Permanent\" ExitDate=\"9999-12-31T00:00:00\" ContractDate=\"2019-03-27T00:00:00\" ExitDateHK=\"2f4e01157c1afb7db9137fbc27dc9f09\" ContractDateHK=\"3ec4c2bd06a9c6dccf82fd1b5080c1a9\" Hashdiff=\"d62812cf3c6f256b5dbcd9047114862b\" scd_start=\"2020-03-01T00:00:00\" scd_end=\"2022-01-05T00:00:00\" scd_version=\"1\" scd_active=\"0\" CostCentreID=\"3\" DepartmentID=\"2\" JobGradeID=\"1\" IntervalFromDateHK=\"9630953f8423d4587a7b88896f72598f\" IntervalToDateHK=\"a712bd324387f05f8e63ed6462cc3f0b\" IntervalToDate=\"2020-10-31T00:00:00\" TaxYear=\"2021\" NormalCashPay=\"3090.00\" TotalPackageValue=\"3090.00\" TotalGrossCashPay=\"3090.00\" TotalNettPay=\"3059.10\" TotalCostToCompany=\"3090.00\" TotalOvertimeHours=\"0.00\" TotalOvertimeValue=\"0.00\" TotalNormalTimeHours=\"173.36\" TotalNormalTimeValue=\"3090.00\" TotalBonuses=\"0.00\" TotalGroupIncome=\"3090.00\" TotalGroupOccasional=\"0.00\" TotalGroupDeductions=\"30.90\" TotalGroupStatutory=\"30.90\" TotalEmployeesTax=\"0.00\" TotalTaxAbatements=\"-30.90\" TotalUIF=\"61.80\" TotalSDL=\"30.90\" UIFRemuneration=\"3090.00\" SDLRemuneration=\"3090.00\" OIDARemuneration=\"3090.00\" />"
                  mediaTypes:
                  - "application/xml"
      fe271c6b-0775-44d0-ad09-201954d7695a:
        path: "/getFacts/template"
        operations:
          "99ba7222-e7d9-4393-961f-fd3a901621ce":
            name: "Test_OP"
            method: "GET"
            responses:
              c5d391a5-b210-4858-bbb3-a609b851e705:
                status: "200"
                bodies:
                - type: "OBJECT"
                  examples:
                  - value: "<facts>singleline</facts>"
                  mediaTypes:
                  - "application/json"
    types:
      "5f4862f9-a1ee-424e-bac7-6676e120628d":
        name: "entry_fact"
        type: "OBJECT"
        examples:
        - value: "<row Schema_hk=\"b29015e368af9e66239f5ac48448b979\" Schema=\"YCOA\" Company_x0020_No=\"110\" Company_hk=\"a87fdcf6948095213d6d2737659d64e7\" Branch_x0020_No=\"1710\" Date=\"2021-01-31T00:00:00\" Date_hk=\"56acd4f269bafddc3987c14f4881bb54\" Period=\"202101\" Year=\"2021\" Month=\"1\" Account_hk=\"ada79b010949af6f7eb709d13110a81f\" Account_x0020_No=\"10010000\" Balance_x0020_Carried_x0020_Forward_x0020_Cn=\"Y\" Balance_x0020_Carried_x0020_Forward=\"-9057.53\" Monthly_x0020_begin_x0020_Balance=\"0.00\" Monthly_x0020_Debit=\"0.00\" Monthly_x0020_Credit=\"0.00\" Monthly_x0020_Balance=\"-9057.53\" Balance=\"-9057.53\" Acceptance_x0020_Cn=\"N\" Acceptance_x0020_Gr=\"10010000\" Account_x0020_Monthly_x0020_Balance=\"-9057.53\" Account_x0020_Balance=\"-9057.53\" Gr_x0020_Monthly_x0020_Balance=\"-9057.53\" Gr_x0020_Balance=\"-9057.53\" Account_x0020_Type=\"Petty Cash\" Account_x0020_Category=\"1\" Account_x0020_Class=\"111100\" Currency_x0020_Cc=\"USD\" Currency_x0020_Gc=\"USD\" Currency_x0020_Coc=\"CHF\" Exchange_x0020_Rate_x0020_Cc_x0020_Gc=\"1.00000\" Exchange_x0020_Rate_x0020_Gc_x0020_Coc=\"0.00000\" Currency_x0020_Dim=\"1\" rec_Load_ts=\"2023-04-12T09:30:26.730\" rec_SourceSystem_str=\"SAP\" />"
      "90705111-8346-4ed1-a84c-754ab2455336":
        name: "account"
        type: "OBJECT"
      bde0b2f2-f2ed-46fd-82b4-1379b0d420c6:
        name: "entry_account"
        type: "#/contract/types/90705111-8346-4ed1-a84c-754ab2455336"
        examples:
        - value: "<row Account_hk=\"c41add98e452e2d672f649ca6cc06ebe\" Company_x0020_No=\"110\" Company_x0020_Area_x0020_No=\"1000\" Branch_x0020_No=\"1010\" Account_x0020_Plan=\"YCOA\" Consolid_x0020_Account_x0020_No=\"111100\" Account_id=\"110_1010_YCOA_10010000\" Account_x0020_No=\"10010000\" Account_x0020_Text=\"Petty Cash\" Account_x0020_Class=\"1\" Account_x0020_Class_x0020_Text=\"B_BILANZ\" Acceptance_x0020_Cn=\"N\" Acceptance_x0020_Gr=\"10010000\" Account_x0020_Type=\"FIN.\" Account_x0020_Category=\"FI\" Liquidity_x0020_Cn=\"N\" Overdraft=\"0.00\" Creation_x0020_Year=\"2\" rec_Load_ts=\"2023-03-30T13:23:06.713\" rec_SourceSystem_str=\"SAP\" />"
      ae8ef632-56f4-4930-ace5-b5ba1ad26274:
        name: "calendar"
        type: "OBJECT"
      "5f7a9686-d775-4a86-8651-db48a1d50f0a":
        name: "entry_calendar"
        type: "#/contract/types/ae8ef632-56f4-4930-ace5-b5ba1ad26274"
        examples:
        - value: "<row Calendar_hk=\"000eff92bb9e1969710c72c5bac2de03\" Date=\"2021-01-02T00:00:00\" Date_int=\"20210102\" Week=\"1\" Year=\"2021\" Month_num=\"1\" Day=\"2\" Quarter_num=\"1\" HalfYear_num=\"1\" Weekday_num=\"6\" Weekday=\"Saturday\" Month=\"January\" Quarter=\"1. Quarter\" Half_x0020_Year=\"1. HalfYear\" Workday=\"0\" rec_Load_ts=\"2023-06-07T10:20:56.823\" rec_SourceSystem_str=\"CORE\" />"
      "50ef1b31-92c7-4e6a-836e-423a8c15a20d":
        name: "costcenter"
        type: "OBJECT"
      "920a4b32-aef4-4c73-8b8b-5b221f6f85c7":
        name: "entry_costcenter"
        type: "#/contract/types/50ef1b31-92c7-4e6a-836e-423a8c15a20d"
        examples:
        - value: "<row CostCentreHK=\"c4ca4238a0b923820dcc509a6f75849b\" CostCentreID=\"1\" CostCentre=\"Austria\" />"
      "2850be16-97e1-4266-bde2-d2e4b01b3909":
        name: "department"
        type: "OBJECT"
      "1acc6d93-458b-41ff-8bca-6eaf06ad5537":
        name: "entry_department"
        type: "#/contract/types/2850be16-97e1-4266-bde2-d2e4b01b3909"
        examples:
        - value: "<row DepartmentHK=\"a87ff679a2f3e71d9181a67b7542122c\" DepartmentID=\"4\" Department=\"Operations\" />"
      d8857aaf-5b5b-4432-aecf-2f93f9338bd7:
        name: "employee"
        type: "OBJECT"
      "745736da-a07b-432a-bdb2-4efeb0db4099":
        name: "entry_employee"
        type: "#/contract/types/d8857aaf-5b5b-4432-aecf-2f93f9338bd7"
        examples:
        - value: "<row EmployeeSK=\"9060\" EmployeeHK=\"20c097b913a26ba121cd74da10e7558f\" EmployeeNumber=\"BC7249\" EntryDate=\"2023-02-01T00:00:00\" CompanyRegNo=\"HICO.00002\" CompanyName=\"HICO Demo \" FirstNames=\"Baby\" Surname=\"Thibela\" CurrentEmployeeStatus=\"Active\" MaritalStatus=\"Single / Never Married\" EmployeeStatus=\"Active\" CurrentStatusEffectiveDate=\"26/02/2023\" Race=\"Coloured\" Gender=\"Male\" Nationality=\"ZAF\" ForeignNational=\"National\" DateOfBirth=\"1970-06-05T00:00:00\" JobGrade=\"Entry-level\" JobGradeHK=\"c4ca4238a0b923820dcc509a6f75849b\" JobGradeEffectiveDate=\"26/02/2023\" JobTitle=\"Clerk\" JobTitleEffectiveDate=\"26/02/2023\" OccupationalLevel=\"Unskilled &amp; Defined Decision Makers\" OccupationalCatagory=\"Service and Sales Workers\" CostCentre=\"Germany\" CostCentreHK=\"c81e728d9d4c2f636f067f89cc14862c\" CostCentreEffectiveDate=\"26/02/2023\" Department=\"Marketing &amp; Sales\" DepartmentHK=\"c81e728d9d4c2f636f067f89cc14862c\" DepartmentEffectiveDate=\"26/02/2023\" EmploymentType=\"Temporary\" ExitDate=\"9999-12-31T00:00:00\" ContractDate=\"2023-02-26T00:00:00\" ExitDateHK=\"2f4e01157c1afb7db9137fbc27dc9f09\" ContractDateHK=\"4a153d17df87bc956ba907b15e68b7cb\" IntervalFromDate=\"2023-02-01T00:00:00\" Hashdiff=\"3d6a5cae11570d5bc416e5e46cfe35aa\" scd_start=\"2023-02-26T00:00:00\" scd_version=\"2\" scd_active=\"1\" />"
      dbed4348-4705-4022-afd1-183122036623:
        name: "grade"
        type: "OBJECT"
      "2cfeee6f-a32c-40c5-a650-117722635a4b":
        name: "entry_grade"
        type: "#/contract/types/dbed4348-4705-4022-afd1-183122036623"
        examples:
        - value: "<row JobGradeHK=\"1679091c5a880faf6fb5e6087eb1b2dc\" JobGradeID=\"6\" JobGrade=\"Senior Management\" />"
      "0b86c562-650b-49bc-a2b2-c13e5b5a7f0d":
        name: "salary"
        type: "OBJECT"
      "157185b0-5fba-4c79-8115-8a852ade5ffe":
        name: "entry_salary"
        type: "#/contract/types/0b86c562-650b-49bc-a2b2-c13e5b5a7f0d"
        examples:
        - value: "<row EmployeeSK=\"1018\" EmployeeHK=\"55507ef387f98cdb7edafe7fa0bdd77f\" EmployeeNumber=\"BC2649\" IntervalFromDateHK=\"9630953f8423d4587a7b88896f72598f\" IntervalFromDate=\"2020-10-01T00:00:00\" IntervalToDateHK=\"a712bd324387f05f8e63ed6462cc3f0b\" IntervalToDate=\"2020-10-31T00:00:00\" TaxYear=\"2021\" CompanyRegNo=\"HICO.00002\" NormalCashPay=\"3090.00\" TotalPackageValue=\"3090.00\" TotalGrossCashPay=\"3090.00\" TotalNettPay=\"3059.10\" TotalCostToCompany=\"3090.00\" TotalOvertimeHours=\"0.00\" TotalOvertimeValue=\"0.00\" TotalNormalTimeHours=\"173.36\" TotalNormalTimeValue=\"3090.00\" TotalBonuses=\"0.00\" TotalGroupIncome=\"3090.00\" TotalGroupOccasional=\"0.00\" TotalGroupDeductions=\"30.90\" TotalGroupStatutory=\"30.90\" TotalEmployeesTax=\"0.00\" TotalTaxAbatements=\"-30.90\" TotalUIF=\"61.80\" TotalSDL=\"30.90\" UIFRemuneration=\"3090.00\" SDLRemuneration=\"3090.00\" OIDARemuneration=\"3090.00\" />"
      "96836d9b-0ec2-4a39-a20c-428b5d22710a":
        name: "balance"
        type: "OBJECT"
      f3375145-7ef0-47bc-a467-63525dbba2ae:
        name: "bilance"
        type: "OBJECT"
      "129b7ac3-0251-4721-83e9-b0a496885cf3":
        name: "employee_all"
        type: "OBJECT"
  components:
    queryParameters:
      ae8679cf-d0fc-454c-9ca3-a828fea3d6f1:
        name: "limit"
        componentName: "limit"
        type: "INTEGER"
        required: false
        default: 0
        examples:
        - value: 100
      "4f57eb34-f444-4263-8348-f611aae1f553":
        name: "offset"
        componentName: "offset"
        type: "INTEGER"
        required: false
        default: 0
        examples:
        - value: 200
api-tryin: |-
  {
    "version" : 6,
    "entities" : [ {
      "entity" : {
        "type" : "Project",
        "name" : "API_Test_GPT 1.0.0",
        "description" : "Keine Beschreibung",
        "importedFrom" : "a347a150-95b3-425a-acc7-8904e8e74613"
      },
      "children" : [ {
        "entity" : {
          "type" : "Request",
          "id" : "8f1c502a-9732-4039-95f3-9b505d54afdf",
          "name" : "/getFacts",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getFacts/",
            "query" : {
              "delimiter" : "&",
              "items" : [ {
                "name" : "limit",
                "value" : "100",
                "enabled" : false
              }, {
                "name" : "offset",
                "value" : "200",
                "enabled" : false
              } ]
            }
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ {
            "enabled" : true,
            "name" : "Accept",
            "value" : "application/json"
          } ],
          "headersType" : "Form",
          "uriEditor" : true
        }
      }, {
        "entity" : {
          "type" : "Request",
          "id" : "54c5c001-9844-4c82-b89d-338578f5860d",
          "name" : "getAccounts",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getDimensions/Accounts",
            "query" : {
              "delimiter" : "&",
              "items" : [ {
                "name" : "limit",
                "value" : "100",
                "enabled" : false
              }, {
                "name" : "offset",
                "value" : "200",
                "enabled" : false
              } ]
            }
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ {
            "enabled" : true,
            "name" : "Accept",
            "value" : "application/xml"
          } ],
          "headersType" : "Form",
          "uriEditor" : true
        }
      }, {
        "entity" : {
          "type" : "Request",
          "id" : "0e945b02-2797-400a-be22-6467e8cf11bf",
          "name" : "getCalendars",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getDimensions/Calendars",
            "query" : {
              "delimiter" : "&",
              "items" : [ {
                "name" : "limit",
                "value" : "100",
                "enabled" : false
              }, {
                "name" : "offset",
                "value" : "200",
                "enabled" : false
              } ]
            }
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ {
            "enabled" : true,
            "name" : "Accept",
            "value" : "application/xml"
          } ],
          "headersType" : "Form",
          "uriEditor" : true
        }
      }, {
        "entity" : {
          "type" : "Request",
          "id" : "1e4fad66-00b9-4da9-9201-0840fa0a8315",
          "name" : "getCostcenters",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getDimensions/Costcenters",
            "query" : {
              "delimiter" : "&",
              "items" : [ {
                "name" : "limit",
                "value" : "100",
                "enabled" : false
              }, {
                "name" : "offset",
                "value" : "200",
                "enabled" : false
              } ]
            }
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ {
            "enabled" : true,
            "name" : "Accept",
            "value" : "application/xml"
          } ],
          "headersType" : "Form",
          "uriEditor" : true
        }
      }, {
        "entity" : {
          "type" : "Request",
          "id" : "cfa2c36b-f716-4ced-a296-58991adae5f5",
          "name" : "getDepartments",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getDimensions/Departments",
            "query" : {
              "delimiter" : "&",
              "items" : [ {
                "name" : "limit",
                "value" : "100",
                "enabled" : false
              }, {
                "name" : "offset",
                "value" : "200",
                "enabled" : false
              } ]
            }
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ {
            "enabled" : true,
            "name" : "Accept",
            "value" : "application/xml"
          } ],
          "headersType" : "Form",
          "uriEditor" : true
        }
      }, {
        "entity" : {
          "type" : "Request",
          "id" : "4e71284d-961e-46bd-b401-4129a76a58ef",
          "name" : "getEmployees",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getDimensions/Employees",
            "query" : {
              "delimiter" : "&",
              "items" : [ {
                "name" : "limit",
                "value" : "100",
                "enabled" : false
              }, {
                "name" : "offset",
                "value" : "200",
                "enabled" : false
              } ]
            }
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ {
            "enabled" : true,
            "name" : "Accept",
            "value" : "application/xml"
          } ],
          "headersType" : "Form",
          "uriEditor" : true
        }
      }, {
        "entity" : {
          "type" : "Request",
          "id" : "da593950-f72b-42dc-b714-7aaaa6f24efc",
          "name" : "getGrades",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getDimensions/Grades",
            "query" : {
              "delimiter" : "&",
              "items" : [ {
                "name" : "limit",
                "value" : "100",
                "enabled" : false
              }, {
                "name" : "offset",
                "value" : "200",
                "enabled" : false
              } ]
            }
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ {
            "enabled" : true,
            "name" : "Accept",
            "value" : "application/xml"
          } ],
          "headersType" : "Form",
          "uriEditor" : true
        }
      }, {
        "entity" : {
          "type" : "Request",
          "id" : "36eb9a25-afbd-460a-bf0b-0cbf9f686bbb",
          "name" : "getSalary",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getDimensions/Salaries",
            "query" : {
              "delimiter" : "&",
              "items" : [ {
                "name" : "limit",
                "value" : "100",
                "enabled" : false
              }, {
                "name" : "offset",
                "value" : "200",
                "enabled" : false
              } ]
            }
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ {
            "enabled" : true,
            "name" : "Accept",
            "value" : "application/xml"
          } ],
          "headersType" : "Form",
          "uriEditor" : true
        }
      }, {
        "entity" : {
          "type" : "Request",
          "id" : "dde1f81d-7738-45b1-81f1-a8d54b3b971d",
          "name" : "getBalance",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getFacts/Balance",
            "query" : {
              "delimiter" : "&",
              "items" : [ {
                "name" : "limit",
                "value" : "100",
                "enabled" : false
              }, {
                "name" : "offset",
                "value" : "200",
                "enabled" : false
              } ]
            }
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ {
            "enabled" : true,
            "name" : "Accept",
            "value" : "application/json"
          } ],
          "headersType" : "Form",
          "uriEditor" : true
        }
      }, {
        "entity" : {
          "type" : "Request",
          "id" : "a42ca501-608d-4687-a306-43ddf6b9e0c8",
          "name" : "getEmployeeSPOT",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getFacts/Employee",
            "query" : {
              "delimiter" : "&",
              "items" : [ {
                "name" : "limit",
                "value" : "100",
                "enabled" : false
              }, {
                "name" : "offset",
                "value" : "200",
                "enabled" : false
              } ]
            }
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ {
            "enabled" : true,
            "name" : "Accept",
            "value" : "application/xml"
          } ],
          "headersType" : "Form",
          "uriEditor" : true
        }
      }, {
        "entity" : {
          "type" : "Request",
          "id" : "99ba7222-e7d9-4393-961f-fd3a901621ce",
          "name" : "Test_OP",
          "uri" : {
            "host" : "${\"BaseUrl\"}",
            "path" : "/getFacts/template"
          },
          "method" : {
            "link" : "",
            "name" : "GET"
          },
          "headers" : [ {
            "enabled" : true,
            "name" : "Accept",
            "value" : "application/json"
          } ],
          "headersType" : "Form"
        }
      } ]
    } ],
    "environments" : [ {
      "name" : "API_Test_GPT 1.0.0",
      "importedFrom" : {
        "projectId" : "a347a150-95b3-425a-acc7-8904e8e74613"
      },
      "variables" : {
        "28cd364c-a4a1-46ba-9416-be7a81d09fb5" : {
          "name" : "BaseUrl",
          "value" : "http://localhost:8090",
          "enabled" : true,
          "private" : false
        }
      }
    } ]
  }
---
