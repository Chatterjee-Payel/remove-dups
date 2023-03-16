# remove-dups
class Solution{
public:
	string removeDuplicates(string str) {
	    // code here
	    unordered_map<char,int>mp;
	   string s="";
	   for(int i=0;i<str.size();i++){
	         if(mp[str[i]]==0)
	         {
	             s+=str[i];
	         }
	         mp[str[i]]++;
	   }
	   return s;
	}
};
