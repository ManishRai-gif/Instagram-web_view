# Instagram-web_view
<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Instagram Desktop UI</title>
   <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
   <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.0/font/bootstrap-icons.css">
   <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  
   <style>
       body {
           background-color: rgb(248, 249, 250);
           font-family: 'Inter', sans-serif;
           color: rgb(33, 37, 41);
       }
       .sidebar {
           background-color: rgb(255, 255, 255);
           height: 100vh;
           border-right: 1px solid rgb(238, 238, 238);
           padding: 40px 25px;
           position: fixed;
           width: inherit;
       }


       .logo {
           font-size: 24px;
           font-weight: 700;
           margin-bottom: 40px;
           display: flex;
           align-items: center;
           gap: 10px;
       }


       .profile-img {
           width: 90px;
           height: 90px;
           border-radius: 50%;
           padding: 4px;
           border: 2px solid rgb(214, 41, 118);
           object-fit: cover;
       }


       .nav-link {
           color: rgb(108, 117, 125);
           font-weight: 500;
           padding: 12px 0;
           display: flex;
           align-items: center;
           gap: 15px;
           text-decoration: none;
       }
       .nav-link.active {
           color: rgb(255, 71, 87);
           border-left: 3px solid rgb(255, 71, 87);
           padding-left: 15px;
           margin-left: -25px;
       }
       .main {
           margin-left: 25%;
           padding: 0;
           background-color: rgb(255, 255, 255);
       }
       .content-area {
           padding: 30px;
       }


       header {
           padding: 20px 30px;
       }
       .search-box {
           background-color: rgb(241, 243, 245);
           border-radius: 12px;
           border: none;
           padding: 10px 20px;
           width: 350px;
       }
       .create {
           background: rgb(255, 107, 107);
           color: white;
           border: none;
           border-radius: 12px;
           padding: 10px 20px;
           font-weight: 600;
       }
       .story-avatar {
           width: 65px;
           height: 65px;
           border-radius: 50%;
           border: 2px solid rgb(214, 41, 118);
           padding: 3px;
       }
       .trending-panel {
           border-left: 1px solid rgb(238, 238, 238);
           padding: 30px;
           height: 100vh;
       }
       .trending-grid {
           display: grid;
           grid-template-columns: 1fr 1fr;
           gap: 10px;
       }
       .trend {
           width: 100%;
           border-radius: 8px;
           aspect-ratio: 1;
           object-fit: cover;
       }


       hr {
           border-top: 1px solid rgb(238, 238, 238);
           opacity: 1;
           margin: 20px 0;
       }
   </style>
</head>
<body>


<div class="container-fluid">
   <div class="row g-0">
      
       <div class="col-md-3">
           <div class="sidebar">
               <div class="logo">
                   <i class="bi bi-instagram"></i> Instagram
               </div>


               <div class="text-center mb-4">
                   <img src="m.png" class="profile-img" alt="Vera">
                   <h5 class="mt-3 mb-0 fw-bold">Vera Cherry</h5>
                   <p class="text-muted small">Bremen, Germany</p>
               </div>


               <div class="d-flex justify-content-around text-center mb-4 small">
                   <div><b>578</b><br><span class="text-muted">POSTS</span></div>
                   <div><b>37.2K</b><br><span class="text-muted">FOLLOWERS</span></div>
                   <div><b>989</b><br><span class="text-muted">FOLLOWING</span></div>
               </div>


               <hr>


               <nav>
                   <a  class="nav-link active"><i class="bi bi-house-door-fill"></i> Feed</a>
                   <a  class="nav-link"><i class="bi bi-compass"></i> Explore</a>
                   <a  class="nav-link"><i class="bi bi-chat-dots"></i> Direct</a>
                   <a class="nav-link"><i class="bi bi-tv"></i> IG TV</a>
                   <a  class="nav-link"><i class="bi bi-graph-up"></i> Stats</a>
                   <a class="nav-link"><i class="bi bi-gear"></i> Settings</a>
               </nav>


               <div style="margin-top: 100px;">
                   <hr>
                   <a  class="nav-link"><i class="bi bi-box-arrow-right"></i> Log out</a>
               </div>
           </div>
       </div>


       <div class="col-md-9 main">
           <header class="d-flex justify-content-between align-items-center">
               <div class="d-flex align-items-center gap-3">
                   <i class="bi bi-search text-muted"></i>
                   <input type="text" class="search-box" placeholder="Search"><i class="bi bi-mic mic-icon"></i>
               </div>
               <div class="d-flex align-items-center gap-3">
                   <button class="btn create"><i class="bi bi-plus-lg"></i> Create now Post</button>
                   <i class="bi bi-send fs-5"></i>
                   <i class="bi bi-bell fs-5"></i>
                   <i class="bi bi-list fs-4"></i>
               </div>
           </header>


           <hr>


           <div class="row g-0">
               <div class="col-md-8 content-area">
                   <div class="d-flex justify-content-between align-items-center mb-4">
                       <h5 class="fw-bold mb-0">Stories</h5>
                       <a  class="text-dark text-decoration-none small fw-bold">Watch all <i class="bi bi-play-fill"></i></a>
                   </div>


                   <div class="d-flex gap-4 mb-5 overflow-hidden">
                       <div class="text-center small"><img src="m.png" class="story-avatar"><br>Add story</div>
                       <div class="text-center small"><img src="m.png" class="story-avatar"><br>Pertdana</div>
                       <div class="text-center small"><img src="m.png" class="story-avatar"><br>Ben Schade</div>
                       <div class="text-center small"><img src="m.png" class="story-avatar"><br>Shubka</div>
                   </div>


                   <div class="d-flex justify-content-between align-items-center mb-3">
                       <h5 class="fw-bold mb-0">Feeds</h5>
                       <div class="d-flex gap-3 small">
                           <span class="text-muted">Latest</span>
                           <span class="fw-bold"><i class="bi bi-circle-fill text-danger small"></i> Popular</span>
                       </div>
                   </div>


                   <div class="card border-0 shadow-sm p-3">
                       <div class="d-flex justify-content-between mb-3">
                           <div class="d-flex align-items-center gap-2">
                               <img src="m.png" class="rounded-circle" width="40" height="40">
                               <div><b class="d-block small">Masidur Rahman</b><small class="text-muted">Bremen, Germany</small></div>
                           </div>
                           <i class="bi bi-three-dots"></i>
                       </div>
                       <img src="m.png" class="img-fluid rounded-4 mb-3" alt="Post">
                       <div class="d-flex justify-content-between">
                           <div class="d-flex gap-4 small">
                               <span><i class="bi bi-heart"></i> 28.5K Like</span>
                               <span><i class="bi bi-chat"></i> 33 Comment</span>
                               <span><i class="bi bi-share"></i> 134 Share</span>
                           </div>
                           <span><i class="bi bi-bookmark"></i> 16 Saved</span>
                       </div>
                   </div>
               </div>


               <div class="col-md-4 trending-panel">
                   <h6 class="fw-bold mb-4">Trending Feeds</h6>
                   <div class="trending-grid mb-5">
                       <img src="m.png" class="trend">
                       <img src="m.png" class="trend">
                       <img src="m.png" class="trend">
                       <img src="m.png" class="trend">
                   </div>


                   <h6 class="fw-bold mb-4">Suggestions for you</h6>
                   <div class="d-flex align-items-center justify-content-between mb-3">
                       <div class="d-flex align-items-center gap-2">
                           <img src="m.png" class="rounded-circle" width="35" height="35">
                           <div><b class="small d-block">Websiteyket</b><small class="text-muted" style="font-size: 10px;">Elk Grove, California</small></div>
                       </div>
                   </div>
                   </div>
           </div>
       </div>
   </div>
</div>


</body>
</html>

