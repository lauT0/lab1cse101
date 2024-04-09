# Sam's User Page

### Background in Computer Science:
Hello, my name is Sam and I'm a second year at UCSD majoring in computer science. Before college I only had some experience with code. I'm glad I made the decision to major in computer science because I ended up _really_ liking it! 
> I'm looking forward to this class as a introduction into software engineering. I'm not exactly sure what field I want to go into, so I'm excited to explore SWE and see if I like it.

### Hobbies:
* Something I really like to do in my free time is drawing. About 2 years ago I started to teach myself digital art using [Krita](https://krita.org/en/) (a free drawing software). Here is some art I have made! ![](drawing.png)
* I also enjoy piano and music, put I haven't played much recently. Hopefully I'll find the time to play again.
* I'm on a mission to watch all the studio ghibli movies. I love the art and and nostoglic feeling they have. My favorite is Howl's Moving Castle and Nausicaä of the Valley of the Wind. I could talk about it forever. In fact, here's a ranking of all the Ghibli movies I watched so far (do you agree?):
  1. Howl's moving castle - 10/10
  2. Nausicaä of the Valley of the Wind - 10/10
  3. spirited away - 8.5/10
  4. The Wind Rises - 8.5/10
  5. Ponyo - 8/10
  6. kiki's delivery service - 8/10
  7. Whisper of the Heart - 6/10
  8. From up on Poppy Hill - 5/10 **weird** 
  9. Ocean waves - 4/10 ***horrible***

### Code Sample:
I'm trying to leetcode more in order to improve my coding skills and I also want to start doing hackathons. This is my solution to leetcode 11. Container With Most Water:

```
class Solution {
public:
    int maxArea(vector<int>& height) {
        int max_vol = 0;
        int i = 0;
        int j = height.size() -1;
        int curr;
        while (i < j){
            curr = min(height[i], height[j]) * (j -i);
            if (curr > max_vol){
                max_vol = curr;
            }
            if (height[i] < height[j]){
                i ++;
            }
            else {j--;}
        }
        return max_vol;
    }
};
```
