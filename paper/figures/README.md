# 图片说明

## 当前图片

- `liang-placeholder.1.pdf`：作者自制的时间线占位图，用于保证论文工程可编译。
- `liang-placeholder.1.tex`：生成该占位图的 TikZ 源文件。

## 替换方法

1. 准备来源和授权清楚的图片文件，例如公开授权照片、馆藏页面明确允许使用的图片，或自行制作的图表。
2. 将图片放入本目录，建议使用无空格的文件名，例如 `liang-authorized-photo.png`。
3. 在 `../main.tex` 中把：

   ```tex
   \includegraphics[width=0.86\textwidth]{liang-placeholder.1.pdf}
   ```

   改为新图片文件名。
4. 同时修改 `figure` 的 `\caption{...}`，写明图片来源、作者/机构、授权或使用许可，以及访问日期或制作日期。
5. 若使用照片，不要只写“网络图片”；必须能追溯到原始页面或正式出版/馆藏信息。

## 目前论文中的处理

当前 PDF 使用占位图，不作为史料证据；正文论证不依赖该图。
