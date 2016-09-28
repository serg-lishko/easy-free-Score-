public class MainActivity extends AppCompatActivity {
    int score = 0;
    int scoreN = 0;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);


    }
    /**
     * This method displays resolts for NY team.
     */
    public void incrementTeamNy1(View view) {
        scoreN = scoreN + 1;
        displayForTeamNy1(scoreN);
    }


    public void incrementTeamNy2(View view) {
        scoreN = scoreN + 2;
        displayForTeamNy2(scoreN);
    }
    private void displayForTeamNy1(int scoreN) {
        TextView scoreView = (TextView) findViewById(R.id.score_team_NY);
        scoreView.setText(String.valueOf(scoreN));
    }
        /**
     * Displays the given score for Team B.
     */


    private void displayForTeamNy2(int scoreN) {
        TextView scoreView = (TextView) findViewById(R.id.score_team_NY);
        scoreView.setText(String.valueOf(scoreN));
    }


    public void increment1(View view) {
        score = score + 1;
        displayForTeamK1(score);
    }

        public void increment3(View view) {
        score = score + 2;
        displayForTeamK2(score);
    }
    private void displayForTeamK1(int score) {
        TextView scoreView = (TextView) findViewById(
                R.id.score_team_K);
        scoreView.setText(String.valueOf(score));
    }
    private void displayForTeamK2(int score) {
        TextView scoreView = (TextView) findViewById(
                R.id.score_team_K);
        scoreView.setText(String.valueOf(score));
    }
    public void resolt(View view) {
        String whoWins = "Kiev is winner!!! ";
        displayMassage(whoWins);
    }
    public void resoltN(View view) {
        String whoWins = "NY is winner!!! ";
        displayMassage(whoWins);
    }
        private void displayMassage(String message) {
            TextView winnerTextView = (TextView) findViewById(R.id.winner_is);
            winnerTextView.setText(message);
        }

    public void refresh(View view) {
        int score = 0;
        int scoreN = 0;
        displayForTeamK1(score);
        displayForTeamK2(score);
        displayForTeamNy1(scoreN);
        displayForTeamNy2(scoreN);
    }
