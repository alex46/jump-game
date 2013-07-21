jump-game
=========

public class Solution {
    public boolean canJump(int[] A) {
        // Start typing your Java solution below
        // DO NOT write main() function
        int maxCover = 0;
        for (int start = 0; start <= maxCover && start < A.length; start++) {
            if (start+A[start] > maxCover) {
                maxCover = start + A[start];
            }
            if (maxCover >= A.length-1) return true;
        }
        return false;
    }
}
