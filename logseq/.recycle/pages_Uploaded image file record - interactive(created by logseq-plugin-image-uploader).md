- #+BEGIN_QUERY
  {:title "Not uploaded images"
    :query [:find (pull ?b [*])
          :where
          [?b :block/page ?p]
          [?p :block/name ?page_name]
          (not [(clojure.string/includes? ?page_name "created by logseq-plugin-image-uploader")])
          [?b :block/content ?content]
          (not [(clojure.string/includes? ?content "{:title \"Not uploaded images\"")])
          [(clojure.string/includes? ?content "](../assets")]
          [(clojure.string/includes? ?content "![")]
          (or [(clojure.string/includes? ?content ".png)")]
              [(clojure.string/includes? ?content ".jpg)")]
              [(clojure.string/includes? ?content ".jpeg)")]
              [(clojure.string/includes? ?content ".gif)")]
              [(clojure.string/includes? ?content ".tiff)")]
              [(clojure.string/includes? ?content ".tif)")]
              [(clojure.string/includes? ?content ".bmp)")]
              [(clojure.string/includes? ?content ".svg)")]
              [(clojure.string/includes? ?content ".webp)")]
              [(clojure.string/includes? ?content ".PNG)")]
              [(clojure.string/includes? ?content ".JPG)")]
              [(clojure.string/includes? ?content ".JPEG)")]
              [(clojure.string/includes? ?content ".GIF)")]
              [(clojure.string/includes? ?content ".TIGG)")]
              [(clojure.string/includes? ?content ".TIF)")]
              [(clojure.string/includes? ?content ".VMP)")]
              [(clojure.string/includes? ?content ".SVG)")]
              [(clojure.string/includes? ?content ".WEBP)")])
        ]}
  #+END_QUERY
	- ![Uploaded by Image Uploder](../assets/image_1665367486378_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665368147072_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665368920907_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665371131177_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665371237672_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665371623737_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665371881171_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665371939941_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665371945207_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665372748191_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665372964438_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665374937673_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665375148863_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665375177063_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665376102513_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665376112179_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665376228626_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665376245571_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665376340689_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665376347692_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665384570027_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665384619870_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665384802947_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665384836722_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665384885330_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665385008006_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665385053271_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665450446516_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665450675442_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665450941609_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665450947513_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665451082964_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665451169104_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665451196231_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665451505236_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665451505236_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665451515445_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665454722607_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665455081839_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665455093091_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665459586402_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665459601015_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665459755533_0.png)
	- ![Uploaded by Image Uploder](../assets/image_1665459794688_0.png)