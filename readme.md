# [Communication Interference] Six Common Communication Interference Signals [with MATLAB Code]

Single-tone jamming is a type of jamming that targets a single frequency point of the target signal, with the interference signal energy concentrated at a fixed frequency. Its expression is as follows:
Multi-tone jamming involves interfering with multiple target frequencies, with the interference signal energy dispersed compared to single-tone jamming. The manifestation is the superposition of multiple single-tone jammings, and its expression is as follows:
Bandwidth noise jamming involves generating noise through a broadband filter in each band width, resulting in noise within each bandwidth.
Narrow-band noise jamming involves the interference signal energy being concentrated in a specific frequency band, with the manifestation being Gaussian white noise, and its expression is as follows:
Comb-like spectrum jamming has similar spectral characteristics to multi-tone jamming, but with spectral peaks arranged at equal intervals and each peak having a certain bandwidth. Its expression is as follows:
Sweep-frequency jamming is a common form of sweep-frequency jamming, where the frequency of the interference signal changes gradually within a certain bandwidth, and its expression is as follows:
% produce a fragment of multiple sinusoid jam\nclear;close all;jnr = 200; % jam-noise ratio\nQ = 10; % number of multiple sinusoid\nPl = 1-0.1*rand(1,Q);                       % Jam power\n​\nFs = 2000;                    % Sampling frequency\nT = 1/Fs;                     % Sample time\nL = 2*Fs;                     % Length of signal\nt = (0:L-1)*T;                % Time vector\n% Sum of a 50 Hz sinusoid\nfs0 = 100;deltafs = 10;\nfs = fs0:deltafs:fs0+(Q-1)*deltafs; % produce same-distance fs\ntheta = 2*pi*rand(1,Q);% random phase\n\n  
% produce a fragment of narrow band noise \nclear;close all;jnr = 20; % jam-noise ratio\nFs = 2000;                    % Sampling frequency\nT = 1/Fs;                     % Sample time\nL = 2*Fs;                     % Length of signal\nt = (0:L-1)*T;                % Time vector\nP=1;% power of noise\ny = wgn(L,1,P); % white noise\n% \n\n​\n​\n  
% produce a fragment of broad band noise \nclear;close all;\nFs = 2000;                    % Sampling frequency\nT = 1/Fs;                     % Sample time\nL = 2*Fs;                     % Length of signal\nt = (0:L-1)*T;                % Time vector\nP=1;% power of noise\ny = wgn(L,1,P/600); % white noise\n% \n% y = awgn(x,jnr,'measured');    % Sinusoids plus noise\n\n  
% produce a fragment of comb-like noise \nclear;close all;\nFs = 2000;                    % Sampling frequency\nT = 1/Fs;                     % Sample time\nL = 2*Fs;                     % Length of signal\nt = (0:L-1)*T;                % Time vector\nP=1;% power of noise\ny = wgn(L,1,P); % white noise\n% \n  
% produce a fragment of scanning frequency jam\nclear;close all;jnr = 1000; % jam-noise ratio\nFs = 2000;                    % Sampling frequency\nT = 1/Fs;                     % Sample time\nL = 2*Fs;                     % Length of signal 2Second\nt = (0:L-1)*T;                % Time vector\nom = 2*pi*10;\nbe = 2*pi*50;\n\n  

## Images

![(Communication Interference)6 Common Communication Interference Signals [with MATLAB Code]](01.jpg)
![(Communication Interference)6 Common Communication Interference Signals [with MATLAB Code]](02.jpg)
![(Communication Interference)6 Common Communication Interference Signals [with MATLAB Code]](03.jpg)
![(Communication Interference)6 Common Communication Interference Signals [with MATLAB Code]](04.jpg)
![(Communication Interference)6 Common Communication Interference Signals [with MATLAB Code]](05.jpg)
![(Communication Interference)6 Common Communication Interference Signals [with MATLAB Code]](06.jpg)
![(Communication Interference)6 Common Communication Interference Signals [with MATLAB Code]](07.jpg)
![(Communication Interference)6 Common Communication Interference Signals [with MATLAB Code]](08.jpg)
![(Communication Interference)6 Common Communication Interference Signals [with MATLAB Code]](09.jpg)
![(Communication Interference)6 Common Communication Interference Signals [with MATLAB Code]](10.jpg)
![(Communication Interference)6 Common Communication Interference Signals [with MATLAB Code]](11.jpg)
![(Communication Interference)6 Common Communication Interference Signals [with MATLAB Code]](12.jpg)
![(Communication Interference)6 Common Communication Interference Signals [with MATLAB Code]](13.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
