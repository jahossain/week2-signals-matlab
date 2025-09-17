# week2-signals-matlab
% Define the time vector for continuous signals
t = -5:0.01:5; % Time from -5 to 5 with a step of 0.01

% Unit Impulse
impulse = zeros(size(t)); % Initialize impulse signal
impulse(t == 0) = 1; % Set the impulse at t = 0
figure; % Create a new figure
subplot(3, 2, 1); % Create a subplot for the impulse signal
plot(t, impulse, 'r', 'LineWidth', 2); % Plot the impulse signal
title('Unit Impulse'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid

% Unit Step
step = t >= 0; % Create step signal (1 for t >= 0, 0 otherwise)
subplot(3, 2, 2); % Create a subplot for the step signal
plot(t, step, 'b', 'LineWidth', 2); % Plot the step signal
title('Unit Step'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid

% Unit Ramp
ramp = t .* (t >= 0); % Create ramp signal (t for t >= 0, 0 otherwise)
subplot(3, 2, 3); % Create a subplot for the ramp signal
plot(t, ramp, 'g', 'LineWidth', 2); % Plot the ramp signal
title('Unit Ramp'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid

% Exponential Signal
exponential = exp(t); % Create exponential signal e^t
subplot(3, 2, 4); % Create a subplot for the exponential signal
plot(t, exponential, 'm', 'LineWidth', 2); % Plot the exponential signal
title('Exponential Signal'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid

% Signum Signal
signum = sign(t); % Create signum signal (-1 for t < 0, 0 for t = 0, 1 for t > 0)
subplot(3, 2, 5); % Create a subplot for the signum signal
plot(t, signum, 'c', 'LineWidth', 2); % Plot the signum signal
title('Signum Signal'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid

% Sinc Signal
sinc_signal = sinc(t); % Create sinc signal (normalized sinc function)
subplot(3, 2, 6); % Create a subplot for the sinc signal
plot(t, sinc_signal, 'k', 'LineWidth', 2); % Plot the sinc signal
title('Sinc Signal'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid

% Adjust layout
sgtitle('Continuous Time Signals'); % Overall title for the figure
% Display the figure
figure;
% Create a new figure for additional analysis or signals
figure;
% Create a new signal for analysis, e.g., a cosine wave
cosineWave = cos(t); % Create cosine signal
subplot(3, 2, 1); % Create a subplot for the cosine wave
plot(t, cosineWave, 'b', 'LineWidth', 2); % Plot the cosine wave
title('Cosine Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the sine wave
sineWave = sin(t); % Create sine signal
subplot(3, 2, 2); % Create a subplot for the sine wave
plot(t, sineWave, 'r', 'LineWidth', 2); % Plot the sine wave
title('Sine Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the tangent wave
tangentWave = tan(t); % Create tangent signal
subplot(3, 2, 3); % Create a subplot for the tangent wave
plot(t, tangentWave, 'm', 'LineWidth', 2); % Plot the tangent wave
title('Tangent Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the cotangent wave
cotangentWave = cot(t); % Create cotangent signal
subplot(3, 2, 4); % Create a subplot for the cotangent wave
plot(t, cotangentWave, 'g', 'LineWidth', 2); % Plot the cotangent wave
title('Cotangent Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the secant wave
secantWave = sec(t); % Create secant signal
subplot(3, 2, 5); % Create a subplot for the secant wave
plot(t, secantWave, 'k', 'LineWidth', 2); % Plot the secant wave
title('Secant Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the cosecant wave
cosecantWave = csc(t); % Create cosecant signal
subplot(3, 2, 6); % Create a subplot for the cosecant wave
plot(t, cosecantWave, 'y', 'LineWidth', 2); % Plot the cosecant wave
title('Cosecant Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Adjust layout for the new figure
sgtitle('Trigonometric Signals'); % Overall title for the figure
% Create a subplot for the tangent wave
tangentWave = tan(t); % Create tangent signal
subplot(3, 2, 3); % Create a subplot for the tangent wave
plot(t, tangentWave, 'm', 'LineWidth', 2); % Plot the tangent wave
title('Tangent Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the cosecant wave
subplot(3, 2, 6); % Create a subplot for the cosecant wave
plot(t, cosecantWave, 'y', 'LineWidth', 2); % Plot the cosecant wave
title('Cosecant Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the secant wave
subplot(3, 2, 5); % Create a subplot for the secant wave
plot(t, secantWave, 'k', 'LineWidth', 2); % Plot the secant wave
title('Secant Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the cosecant wave
subplot(3, 2, 6); % Create a subplot for the cosecant wave
plot(t, cosecantWave, 'y', 'LineWidth', 2); % Plot the cosecant wave
title('Cosecant Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a new figure for additional analysis or signals
figure;
% Create a new signal for analysis, e.g., a square wave
squareWave = square(t); % Create square signal
subplot(3, 2, 1); % Create a subplot for the square wave
plot(t, squareWave, 'c', 'LineWidth', 2); % Plot the square wave
title('Square Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the triangular wave
triangularWave = sawtooth(t, 0.5); % Create triangular signal
subplot(3, 2, 2); % Create a subplot for the triangular wave
plot(t, triangularWave, 'm', 'LineWidth', 2); % Plot the triangular wave
title('Triangular Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the sawtooth wave
subplot(3, 2, 3); % Create a subplot for the sawtooth wave
plot(t, triangularWave, 'b', 'LineWidth', 2); % Plot the triangular wave
title('Triangular Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the sawtooth wave
subplot(3, 2, 4); % Create a subplot for the sawtooth wave
plot(t, sawtooth(t), 'r', 'LineWidth', 2); % Plot the sawtooth wave
title('Sawtooth Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the sine wave
sineWave = sin(t); % Create sine signal
subplot(3, 2, 5); % Create a subplot for the sine wave
plot(t, sineWave, 'b', 'LineWidth', 2); % Plot the sine wave
title('Sine Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the cosine wave
cosineWave = cos(t); % Create cosine signal
subplot(3, 2, 6); % Create a subplot for the cosine wave
plot(t, cosineWave, 'g', 'LineWidth', 2); % Plot the cosine wave
title('Cosine Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the tangent wave
subplot(3, 2, 4); % Create a subplot for the tangent wave
plot(t, tangentWave, 'm', 'LineWidth', 2); % Plot the tangent wave
title('Tangent Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid
% Create a subplot for the secant wave
subplot(3, 2, 6); % Create a subplot for the secant wave
plot(t, secantWave, 'k', 'LineWidth', 2); % Plot the secant wave
title('Secant Wave'); % Title for the plot
xlabel('Time (s)'); % X-axis label
ylabel('Amplitude'); % Y-axis label
grid on; % Enable grid

![image](https://github.com/jahossain/week2-signals-matlab/blob/main/Images/Screenshot%202025-09-17%20135807.png)
![image](https://github.com/jahossain/week2-signals-matlab/blob/main/Images/Screenshot%202025-09-17%20135848.png)
![image](https://github.com/jahossain/week2-signals-matlab/blob/main/Images/Screenshot%202025-09-17%20135911.png)

# description
The unit impulse is a spike at 𝑡=0t=0, used to test system responses. The unit step switches from 0 to 1 at 𝑡=0t=0, while the unit ramp grows linearly for 𝑡≥0t≥0. The exponential signal either decays or grows exponentially, modeling many natural processes. The signum signal indicates the sign of time (−1, 0, or +1). The sinc signal is an oscillatory, decaying function sin(𝜋𝑡)/(𝜋𝑡)sin(πt)/(πt), important in signal processing and Fourier analysis.
