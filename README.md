# GIS_Covid19_France
Phân tích bộ dữ liệu được xử dụng trong dự án:
- Đầu tiên sẽ có các file dữ liệu sau:
  + data-hospital-covid19-2020-04-13-19h00.csv
  + demographie.csv
  + departements-avec-outre-mer.geojson
  + TCRD_021.csv

- Giải thích bộ dữ liệu (data-hospital-covid19-2020-04-13-19h00.csv)
  + Với bộ dữ liệu này ta có các cột:
    * **sexe : Giới tính**
    * **jour: Ngày mà dữ liệu được cung cấp** 
    * **hosp: Số người hiện đang nằm viện** 
    * **rea: Số người đang hồi sức hoặc được chăm sóc tích cực** 
    * **rad: Số bệnh nhân đã trở về nhà** 
    * **dc: Số bệnh nhân đã mất tại viện** 
    
- Giải thích bộ dữ liệu (demographie.csv)
  + Đây là bộ dữ liệu phân bố dân số, mật độ dân số và diện tích
  + Nguồn dữ liệu tham khảo từ: https://www.regions-et-departements.fr/departements-francais
  + Các cột và ý nghĩa:
    * **code : Vùng**
    * **nom: Tên của vùng** 
    * **Superficie: Diện tích** 
    * **Population: Dân số** 
    * **Densite: Mật độ** 
    
- Giải thích bộ dữ liệu (epartements-avec-outre-mer.geojson)
  + Đây là bộ dữ liệu địa lý của Pháp đã được xây dựng sẵn bao gồm các tọa độ và các type là đối tượng hình học (Polygon, Multipolygon)
  + Nguồn tham khảo: https://github.com/gregoiredavid
  
- Giải thích bộ dữ liệu (TCRD_021.csv)
  + Đây là bộ dữ liệu về phân bổ dân số theo từng vùng
  + Chi tiết các cột:
    * **Cột không tên [0] : Mã vùng(code)**
    * **Cột không tên [1] : Tên vùng**
    * **Ensemble : Tổng dân số trong vùng**
    * **Part des femmes (en %) : Phần trăm nữ giới**
    * **Part des hommes (en %) : Phần trăm nam giới**
    * **Part des 0 à 24 ans (en %) : Phần trăm dân số độ tuổi từ 0 -> 24**
    * **Part des 25 à 59 ans (en %) : Phần trăm dân số độ tuổi từ 25 -> 59**
    * **Part des 60 ans ou plus (en %) : Phần trăm dân số độ tuổi trên 60**
    * **dont part des 75 ans ou plus (en %) : Phần trăm dân số độ tuổi trên 75**
    
 Trong dự án này có sử dụng thư viện KeplerGl nguồn tham khảo: https://docs.kepler.gl/docs/keplergl-jupyter
 ---> Trên đây là thư viện và dữ liệu được xử dụng trong dự án này. Các dữ liệu sẽ được phân chia theo ngày và kết nối qua mã vùng => có được bản đồ của từng ngày.
