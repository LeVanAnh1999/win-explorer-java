win-explorer-java

Tên SV : Lê Văn Ánh

Lớp : 17IT2

Mã SV : 17IT041

Email : lvanh.17it2@sict.udn.vn
Link video hướng dẫn sử dụng : https://youtu.be/mBCQ7h3iAww

Đề 015

  Câu 1:  Thiết kế giao diện phần mềm file Explore.

  Câu 2: Thực hiện chức năng mở thư mục(Open Folder).
  
  Chức năng bổ sung: chức năng xóa File( Delete File).

Cách chạy code:

   1.Tải project từ github

   2.Mở cmd

   3.Dùng lệnh cd chuyển đến thư mục chứa source code

      Ví dụ: cd C:\Users\PC\eclipse-workspace\fileexplorer\src
   4.Biên dịch bằng lệnh javac:

      javac fileexplorer\FileExplorer.java
   5.Chạy bằng lệnh java:

      java fileexplorer.FileExplorer

Biên dịch các dòng lệnh:

-public Container getGui():

Hiển thị các thành phần và chức năng của phần mềm

 -public void showRootFile():

Hiển thị các tệp lên jtree và jtable từ lớp FileTableModel.

  -private void showErrorMessage():

Hàm dùng để hiển thị tin nhắn báo lỗi

  -private void setTableData(final File[] files):

Dùng để cài đặt dự liệu cho table

  -private void setColumnWidth(int column, int width):

Dùng để cài đặt kích cỡ cho table
  
  -private void showChildren(final DefaultMutableTreeNode node):

Hiển thị các cành con của Tree
  
  -private void setFileDetails(File file):

Cài đặt thông tin cho file
  
  -class FileTableModel extends AbstractTableModel

Thực hiện chứ năng hiển thị các cột thông tin lên Table
  
  -public Component getTreeCellRendererComponent():

Thực hiện chức năng cài đặt icon, tên file và lấy đường dẫn cho các Node của JTree

  -public Object getValueAt(int row, int column):

Thực hiện chức năng cài đặt thông tin cho các file
  
   -private void deleteFile()
 
 Thực hiện chức năng xóa File
    -private JButton OppenFolder;
  Nút mở thư mục
    private JButton deleteFile;
  Nút xóa File



HƯỚNG DẪN SỬ DỤNG:

Mở các thư mục bằng cách click 2 lần vào thư mục trong JTree

Chức năng chính:
Mở tập tin:

Chọn thư mục cần mở

Sau đó: click vào "OpenFolder"

Chức năng làm thêm:




Xóa File

Kích chuột vào file muốn xóa

Nhấn nút Delete

Xuất hiện hộp thoại "Are you sure you want to delete this file?" , nhấn OK để xác nhận xóa file, nhấn No để hủy thao tác
