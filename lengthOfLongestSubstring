class Solution {
    public static int lengthOfLongestSubstring(String s) {
        String subs = "";
		String st = "";
		int subsLen = 0;
        for(int i=0; i< s.length(); i++){
			char ch = s.charAt(i);
			if(st.indexOf(ch) == -1){
				st += Character.toString(ch);
            }else if(st.indexOf(ch) > -1){
				if(subs.length() < st.length()){
					subs = st;
					subsLen = subs.length();
					st = Character.toString(ch); 
				}
			}
		}
        if(st != "" && subsLen == 0){
            subsLen = st.length();
        }
		return subsLen;
    }
    
    public static void main(String args[]){
        System.out.println(lengthOfLongestSubstring(" "));
    }
}
