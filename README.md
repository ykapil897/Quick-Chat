<body>
    <h1>Chatting Application</h1>
    <p>
        A lightweight and efficient <strong>real-time chat application</strong> built using 
        <strong>Spring Boot</strong>, <strong>WebSockets</strong>, <strong>SockJS</strong>, and 
        <strong>STOMP Client</strong>. The project delivers fast, reliable, and scalable communication 
        with graceful fallback support—ensuring users stay connected under all network conditions.
    </p>

<hr>

<h2>✨ Features</h2>
<ul>
    <li>Instant, real-time text messaging between connected users.</li>
    <li>High-speed, full-duplex communication via <strong>WebSockets</strong>.</li>
    <li>Automatic fallback with <strong>SockJS</strong> for environments without native WebSocket support.</li>
    <li>Clean, responsive UI designed to enhance the chatting experience.</li>
    <li>Robust and scalable backend powered by <strong>Spring Boot</strong>.</li>
</ul>

<hr>

<h2>🧰 Technologies Used</h2>

<h3>Backend</h3>
<ul>
    <li><strong>Spring Boot</strong>: Handles REST endpoints and WebSocket configuration.</li>
    <li><strong>WebSockets</strong>: Provides low-latency real-time communication.</li>
    <li><strong>SockJS</strong>: Ensures compatibility in environments where WebSockets are blocked or unsupported.</li>
    <li><strong>STOMP</strong>: Adds a structured messaging layer over WebSockets.</li>
</ul>

<hr>

<h2>📐 System Design</h2>
<p>
    The application architecture relies on a <strong>Spring Boot WebSocket server</strong> that manages 
    real-time connections. Clients interact using the <strong>STOMP protocol</strong>, which ensures clean 
    and organized messaging channels. When WebSockets aren’t available, <strong>SockJS</strong> 
    automatically takes over to maintain seamless communication.
</p>

<h3>📊 Diagram</h3>
<p>This system design diagram visualizes the end-to-end communication workflow:</p>
<img src="img.png" alt="System Design Diagram">

<hr>

<h2>🚀 Project Setup</h2>

<h3>Backend Setup</h3>
<ol>
    <li>Clone the repository:
        <pre><code>git clone &lt;repository-url&gt;</code></pre>
    </li>
    <li>Navigate to the backend directory:
        <pre><code>cd backend</code></pre>
    </li>
    <li>Build and run the Spring Boot application:
        <pre><code>./mvnw spring-boot:run</code></pre>
    </li>
</ol>

<hr>

<h2>⚙️ How It Works</h2>
<ol>
    <li><strong>Connection Establishment</strong>:
        <p>Clients initiate a connection to the WebSocket server. If WebSockets aren’t supported, SockJS automatically provides a compatible fallback transport, while STOMP manages subscription and messaging channels.</p>
    </li>
    <li><strong>Messaging</strong>:
        <p>Messages sent by users are transmitted over the WebSocket channel and routed by the backend to subscribed users or chat rooms in real time.</p>
    </li>
    <li><strong>Fallback Mechanism</strong>:
        <p>In restrictive or outdated environments, SockJS maintains communication using HTTP-based transports, ensuring uninterrupted messaging.</p>
    </li>
</ol>

<hr>

<h2>🤝 Contributing</h2>
<p>
    Contributions are highly appreciated!  
    Fork the repository, enhance the application, and submit a pull request to share your improvements.
</p>

</body>
