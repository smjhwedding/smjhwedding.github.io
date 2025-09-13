# smjhwedding.github.io

(처음 한 번) PowerShell에서 설치:

winget install -e --id ImageMagick.ImageMagick

# ① ImageMagick 실행 파일 경로 변수
$IM = "C:\Program Files\ImageMagick-7.1.2-Q16-HDRI\magick.exe"

# ② 히어로 이미지 → WebP/AVIF 3종씩
& $IM "KakaoTalk_20250907_195152669.jpg" -strip -resize 1920x -quality 82 hero-1920.webp
& $IM "KakaoTalk_20250907_195152669.jpg" -strip -resize 1280x -quality 82 hero-1280.webp
& $IM "KakaoTalk_20250907_195152669.jpg" -strip -resize 768x  -quality 82 hero-768.webp

& $IM "KakaoTalk_20250907_195152669.jpg" -strip -resize 1920x -quality 45 hero-1920.avif
& $IM "KakaoTalk_20250907_195152669.jpg" -strip -resize 1280x -quality 45 hero-1280.avif
& $IM "KakaoTalk_20250907_195152669.jpg" -strip -resize 768x  -quality 45 hero-768.avif

# ③ 갤러리 1 → WebP/AVIF 3종
& $IM "KakaoTalk_20250908_010410211_01.jpg" -strip -resize 1024x -quality 82 gallery1-1024.webp
& $IM "KakaoTalk_20250908_010410211_01.jpg" -strip -resize 768x  -quality 82 gallery1-768.webp
& $IM "KakaoTalk_20250908_010410211_01.jpg" -strip -resize 512x  -quality 82 gallery1-512.webp

& $IM "KakaoTalk_20250908_010410211_01.jpg" -strip -resize 1024x -quality 45 gallery1-1024.avif
& $IM "KakaoTalk_20250908_010410211_01.jpg" -strip -resize 768x  -quality 45 gallery1-768.avif
& $IM "KakaoTalk_20250908_010410211_01.jpg" -strip -resize 512x  -quality 45 gallery1-512.avif

# ④ 갤러리 2 → WebP/AVIF 3종
& $IM "KakaoTalk_20250908_010410211.jpg" -strip -resize 1024x -quality 82 gallery2-1024.webp
& $IM "KakaoTalk_20250908_010410211.jpg" -strip -resize 768x  -quality 82 gallery2-768.webp
& $IM "KakaoTalk_20250908_010410211.jpg" -strip -resize 512x  -quality 82 gallery2-512.webp

& $IM "KakaoTalk_20250908_010410211.jpg" -strip -resize 1024x -quality 45 gallery2-1024.avif
& $IM "KakaoTalk_20250908_010410211.jpg" -strip -resize 768x  -quality 45 gallery2-768.avif
& $IM "KakaoTalk_20250908_010410211.jpg" -strip -resize 512x  -quality 45 gallery2-512.avif
