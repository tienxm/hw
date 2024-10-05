### Mermaid
```mermaid
gantt
    title A Gantt Diagram

    section Section
    研擬計畫             :a1, 2024-09-30, 1d
    任務分配             :a2, after a1  , 4d
    取得硬體             :a3, after a1  , 17d
    程式開發             :a4, after a2  , 70d
    安裝硬體             :a5, after a3  , 10d
    程式測試             :a6, after a4  , 30d
    撰寫使用手冊          :a7, after a5  , 25d
    轉換檔案             :a8, after a5  , 20d
    系統測試             :a9, after a6  , 25d
    使用者訓練           :a10, after a7 a8  , 20d
    使用者測試           :a11, after a9 a10  , 25d
```

&nbsp;
&nbsp;

mermaid
graph TD;
    A[編號1:研擬計劃<br/>開始: 2024-09-30<br/>結束: 2024-09-30] -->|1天| B[編號2:任務分配<br/>開始: 2024-09-30<br/>結束: 2024-10-04];
    A -->|1天| C[編號3:取得硬體<br/>開始: 2024-09-30<br/>結束: 2024-10-17];
    B -->|4天| D[編號4:程式開發<br/>開始: 2024-10-05<br/>結束: 2024-12-26];
    C -->|17天| E[編號5:安裝硬體<br/>開始: 2024-10-18<br/>結束: 2024-10-27];
    D -->|70天| F[編號6:程式測試<br/>開始: 2024-12-27<br/>結束: 2025-01-25];
    E -->|10天| G[編號7:撰寫使用手冊<br/>開始: 2024-10-28<br/>結束: 2024-12-01];
    E -->|20天| H[編號8:轉換檔案<br/>開始: 2024-10-28<br/>結束: 2024-12-15];
    F -->|30天| I[編號9:系統測試<br/>開始: 2025-01-26<br/>結束: 2025-02-25];
    G -->|25天| J[編號10:使用者訓練<br/>開始: 2024-12-02<br/>結束: 2024-12-26];
    H -->|20天| J;
    I -->|25天| K[編號11:使用者測試<br/>開始: 2025-02-26<br/>結束: 2025-03-02];
    J -->|20天| K;

    style A fill:#ffcccc,stroke:#333,stroke-width:2px;
    style D fill:#ffcccc,stroke:#333,stroke-width:2px;
    style F fill:#ffcccc,stroke:#333,stroke-width:2px;
    style I fill:#ffcccc,stroke:#333,stroke-width:2px;
    style K fill:#ffcccc,stroke:#333,stroke-width:2px;
<p align="center">關鍵路徑 1>2>4>6>9>11</p>
