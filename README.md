# algorithm_coding_tip


##Making priority queue
###Asssign
priority_queue<pair<int,int> , vector<pair<int,int> >,cmp> pq;

###Make cmp
struct cmp {
	bool operator()(pair<int,int> a, pair<int,int> b) {
		if(a.first>b.first) return true;
		else if(a.first == b.first) {
			if(a.second > b.second) return true;
		}
		return false;
	}
};

###USE
pq.push();
pq.pop();
