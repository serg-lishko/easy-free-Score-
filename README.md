# easy-free-Score-
How to count score
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
