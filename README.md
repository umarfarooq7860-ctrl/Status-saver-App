Feature	Why it matters	Implementation tip
1. Auto-load all statuses	Shows images + videos from .Statuses without manual refresh	Use FileObserver or SwipeRefreshLayout to detect new files
2. Separate Images/Videos tabs	Better UX, faster browsing	TabLayout + ViewPager2 with 2 fragments filtering by .jpg/.mp4
3. One-tap save	Main feature	Copy file to /StatusSaver + MediaScannerConnection.scanFile()
4. Multi-select + save all	Users want to bulk download	RecyclerView with SelectionTracker or checkboxes
5. Built-in player/preview	Let users view before saving	ExoPlayer for video, PhotoView library for zoomable images
6. Direct share to WhatsApp	Share without saving first	Intent.ACTION_SEND with FileProvider URI
7. Repost to WhatsApp status	Popular feature	Same share intent targeting com.whatsapp package
