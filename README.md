---


---

<h1 id="bài-tập-so-sánh-trade-off-các-giải-pháp-prompting-trong-học-tập-và-nghiên-cứu"><strong>BÀI TẬP: SO SÁNH TRADE-OFF CÁC GIẢI PHÁP PROMPTING TRONG HỌC TẬP VÀ NGHIÊN CỨU</strong></h1>
<h2 id="bước-1-đề-xuất-2-prompt-mẫu"><strong>1. Bước 1: Đề xuất 2 prompt mẫu</strong></h2>
<h3 id="giải-pháp-1-prompt-đơn-giản"><strong>Giải pháp 1: Prompt đơn giản</strong></h3>
<p>Bạn là AI gia sư. Hãy giải thích kiến thức theo phương pháp Feynman bằng ngôn ngữ dễ hiểu, có ví dụ thực tế. Sau đó, chấm bài của sinh viên theo Rubric được cung cấp, nêu điểm số, ưu điểm, nhược điểm và cách cải thiện. Nếu thiếu bài làm hoặc Rubric, hãy yêu cầu bổ sung.</p>
<h3 id="giải-pháp-2-prompt-chi-tiết"><strong>Giải pháp 2: Prompt chi tiết</strong></h3>
<p>Bạn là AI gia sư chuyên nghiệp, sử dụng phương pháp Feynman và Rubric để hỗ trợ học tập.</p>
<p>Yêu cầu:</p>
<ol>
<li>Giải thích kiến thức đơn giản, phù hợp với trình độ sinh viên.</li>
<li>Đưa ra ví dụ thực tế.</li>
<li>Đặt 3 câu hỏi kiểm tra kiến thức.</li>
<li>Chấm bài theo từng tiêu chí Rubric.</li>
<li>Giải thích lý do được điểm và mất điểm.</li>
<li>Đưa ra nhận xét và hướng cải thiện.</li>
</ol>
<p>Quy tắc xử lý lỗi:</p>
<ul>
<li>Nếu thiếu bài làm, không chấm điểm.</li>
<li>Nếu thiếu Rubric, yêu cầu bổ sung.</li>
<li>Nếu dữ liệu trống hoặc sai định dạng, thông báo lỗi.</li>
<li>Không tự ý thay đổi thang điểm.</li>
<li>Không tự bịa thông tin.</li>
<li>Tổng điểm phải đúng với Rubric.</li>
</ul>
<p>Đầu ra gồm: Giải thích Feynman, câu hỏi kiểm tra, bảng điểm Rubric, nhận xét và tổng kết.</p>
<h2 id="bước-2-bảng-so-sánh-trade-off"><strong>2. Bước 2: Bảng so sánh Trade-off</strong></h2>

<table>
<thead>
<tr>
<th>Tiêu chí</th>
<th>Giải pháp 1 (Đơn giản)</th>
<th>Giải pháp 2 (Chi tiết)</th>
</tr>
</thead>
<tbody>
<tr>
<td>Độ dễ hiểu</td>
<td>Cao</td>
<td>Trung bình</td>
</tr>
<tr>
<td>Tốn token</td>
<td>Ít</td>
<td>Nhiều hơn</td>
</tr>
<tr>
<td>Tốc độ xử lý</td>
<td>Nhanh</td>
<td>Chậm hơn</td>
</tr>
<tr>
<td>Chặn lỗi dữ liệu</td>
<td>Trung bình</td>
<td>Rất tốt</td>
</tr>
<tr>
<td>Độ chính xác</td>
<td>Khá</td>
<td>Cao hơn</td>
</tr>
<tr>
<td>Dễ sử dụng</td>
<td>Rất dễ</td>
<td>Cần nhập đủ dữ liệu</td>
</tr>
<tr>
<td>Khả năng kiểm soát</td>
<td>Thấp</td>
<td>Cao</td>
</tr>
</tbody>
</table><h2 id="bước-3-lựa-chọn-và-chạy-thử"><strong>3. Bước 3: Lựa chọn và chạy thử</strong></h2>
<p><strong>Phương án lựa chọn: Giải pháp 2.</strong></p>
<p><strong>Lý do:</strong></p>
<ul>
<li>Có hướng dẫn rõ ràng cho AI.</li>
<li>Kiểm soát lỗi dữ liệu tốt hơn.</li>
<li>Chấm điểm theo Rubric cụ thể.</li>
<li>Kết quả đầy đủ và dễ đánh giá.</li>
</ul>
<h3 id="kết-quả-chạy-thử"><strong>Kết quả chạy thử</strong></h3>
<p><strong>Input:</strong></p>
<ul>
<li>Chủ đề: Mạng máy tính.</li>
<li>Bài làm: Mạng máy tính là hệ thống kết nối nhiều máy tính để trao đổi dữ liệu.</li>
<li>Rubric:
<ul>
<li>Đúng kiến thức: 4 điểm.</li>
<li>Giải thích: 3 điểm.</li>
<li>Ví dụ: 2 điểm.</li>
<li>Trình bày: 1 điểm.</li>
</ul>
</li>
</ul>
<p><strong>Output:</strong></p>

<table>
<thead>
<tr>
<th>Tiêu chí</th>
<th>Điểm tối đa</th>
<th>Điểm đạt</th>
</tr>
</thead>
<tbody>
<tr>
<td>Đúng kiến thức</td>
<td>4</td>
<td>4</td>
</tr>
<tr>
<td>Giải thích</td>
<td>3</td>
<td>3</td>
</tr>
<tr>
<td>Ví dụ</td>
<td>2</td>
<td>0</td>
</tr>
<tr>
<td>Trình bày</td>
<td>1</td>
<td>1</td>
</tr>
<tr>
<td><strong>Tổng</strong></td>
<td><strong>10</strong></td>
<td><strong>8</strong></td>
</tr>
</tbody>
</table><p><strong>Nhận xét:</strong></p>
<ul>
<li>Ưu điểm: Kiến thức đúng, trình bày dễ hiểu.</li>
<li>Nhược điểm: Chưa có ví dụ thực tế.</li>
<li>Cải thiện: Bổ sung ví dụ về mạng máy tính trong phòng học.</li>
</ul>

