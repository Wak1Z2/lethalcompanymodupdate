- 22.0.5 : forgot to include 2 line changes in the 22.0.4 build

- 22.0.4 : overtime was still off by 15$

- 22.0.3 : reverted the overtime change, and resyncs the sold value after the items are taken to mitigate value desync

- 22.0.2 : changed how overtime is calculated (edge case where the last day -15$ penalty isn't applied if you already sold some items on any other day)

- 22.0.1 : fixed quota desync for non-host clients

- 22.0.0 : flawless version that totally didn't need immediate fixing