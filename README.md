# magic-submissions
class Student
{
    static const int NUM_SCORES = 5;
    
    int scores[NUM_SCORES];
    
    public:
    
        void input()
        {
            for (int i= 0; i < NUM_SCORES && cin >> scores[i]; i++);
        }
        
        int calculateTotalScore() const
        {
            int sum = 0, i = NUM_SCORES - 1;
            for( ; i >= 0; sum += scores[i--] );
            return sum;
        }
};
