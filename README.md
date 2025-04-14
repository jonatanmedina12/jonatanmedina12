<!-- Aquí está el código SVG para una terminal interactiva en tu README.md de GitHub -->
<svg fill="none" viewBox="0 0 800 400" width="800" height="400" xmlns="http://www.w3.org/2000/svg">
  <foreignObject width="100%" height="100%">
    <div xmlns="http://www.w3.org/1999/xhtml">
      <style>
        .container {
          background-color: #0d1117;
          border-radius: 10px;
          padding: 20px;
          font-family: Arial, Helvetica, sans-serif;
          display: flex;
          flex-direction: column;
          align-items: center;
          justify-content: center;
          margin: 0;
          width: 100%;
          height: 400px;
          overflow: hidden;
        }

        .terminal {
          width: 90%;
          height: 340px;
          background-color: #161b22;
          border-radius: 8px;
          padding: 10px;
          overflow: hidden;
          box-shadow: 0 10px 30px -8px rgba(0, 0, 0, 0.5);
        }

        .terminal-header {
          display: flex;
          align-items: center;
          padding: 5px;
          border-bottom: 1px solid #21262d;
        }

        .terminal-buttons {
          display: flex;
        }

        .btn {
          width: 12px;
          height: 12px;
          border-radius: 50%;
          margin-right: 8px;
        }

        .btn-red {
          background-color: #ff5f56;
        }

        .btn-yellow {
          background-color: #ffbd2e;
        }

        .btn-green {
          background-color: #27c93f;
        }

        .terminal-title {
          flex-grow: 1;
          color: #8b949e;
          text-align: center;
          font-size: 14px;
          font-weight: bold;
        }

        .terminal-body {
          color: #e6edf3;
          font-family: "Courier New", Courier, monospace;
          font-size: 14px;
          line-height: 1.5;
          padding: 10px;
          height: calc(100% - 40px);
          overflow-y: auto;
        }

        .command-line {
          display: flex;
          margin-bottom: 10px;
          align-items: center;
        }

        .prompt {
          color: #7ee787;
          margin-right: 8px;
          flex-shrink: 0;
        }

        .directory {
          color: #58a6ff;
          margin-right: 8px;
          flex-shrink: 0;
        }

        .cursor {
          background-color: #58a6ff;
          animation: blink 1s step-start infinite;
          width: 8px;
          height: 16px;
          position: relative;
          top: 2px;
        }

        @keyframes blink {
          0%, 100% { opacity: 1; }
          50% { opacity: 0; }
        }

        .command {
          white-space: pre-wrap;
          color: #e6edf3;
          flex-grow: 1;
        }

        .output {
          margin-bottom: 15px;
          white-space: pre-wrap;
          color: #8b949e;
        }

        .highlight {
          color: #ff7b72;
        }

        .highlight-blue {
          color: #79c0ff;
        }

        .highlight-green {
          color: #7ee787;
        }

        .highlight-yellow {
          color: #ffa657;
        }

        /* Animación de escritura */
        .typing {
          animation: typing 4s steps(60, end) infinite;
          white-space: nowrap;
          overflow: hidden;
          width: 0;
          max-width: 600px;
          display: inline-block;
        }

        @keyframes typing {
          from { width: 0 }
          to { width: 100% }
        }
      </style>

      <div class="container">
        <div class="terminal">
          <div class="terminal-header">
            <div class="terminal-buttons">
              <div class="btn btn-red"></div>
              <div class="btn btn-yellow"></div>
              <div class="btn btn-green"></div>
            </div>
            <div class="terminal-title">developer-terminal -- /home/tu-usuario</div>
          </div>
          <div class="terminal-body">
            <div class="command-line">
              <span class="prompt">$</span>
              <span class="directory">~/proyectos</span>
              <span class="command typing">ls -la</span>
            </div>
            <div class="output">total 24
drwxr-xr-x  6 usuario  staff  192 Abr 13 14:32 <span class="highlight-blue">.</span>
drwxr-xr-x  7 usuario  staff  224 Abr 13 14:30 <span class="highlight-blue">..</span>
-rw-r--r--  1 usuario  staff  284 Abr 13 14:31 <span class="highlight-blue">.gitignore</span>
drwxr-xr-x 12 usuario  staff  384 Abr 13 14:33 <span class="highlight-green">angular-project</span>
drwxr-xr-x 15 usuario  staff  480 Abr 13 14:32 <span class="highlight-green">react-app</span>
drwxr-xr-x 10 usuario  staff  320 Abr 13 14:30 <span class="highlight-green">spring-api</span></div>
            
            <div class="command-line">
              <span class="prompt">$</span>
              <span class="directory">~/proyectos</span>
              <span class="command typing">cat perfil.json</span>
            </div>
            <div class="output">{
  <span class="highlight-yellow">"nombre"</span>: <span class="highlight">"Tu Nombre"</span>,
  <span class="highlight-yellow">"título"</span>: <span class="highlight">"Desarrollador Full Stack"</span>,
  <span class="highlight-yellow">"habilidades"</span>: [
    <span class="highlight">"Angular"</span>, <span class="highlight">"React"</span>, <span class="highlight">"TypeScript"</span>,
    <span class="highlight">"Spring Boot"</span>, <span class="highlight">".NET"</span>, <span class="highlight">"Python/Django"</span>,
    <span class="highlight">"SOLID"</span>, <span class="highlight">"Clean Code"</span>, <span class="highlight">"DRY"</span>
  ],
  <span class="highlight-yellow">"contacto"</span>: <span class="highlight">"tu-email@ejemplo.com"</span>
}</div>
            
            <div class="command-line">
              <span class="prompt">$</span>
              <span class="directory">~/proyectos</span>
              <span class="command typing">npm run build</span>
            </div>
            <div class="output"><span class="highlight-green">✓</span> Compiled successfully!
<span class="highlight-green">✓</span> 248 modules bundled
<span class="highlight-green">✓</span> Build completed in 4.32s</div>
            
            <div class="command-line">
              <span class="prompt">$</span>
              <span class="directory">~/proyectos</span>
              <span class="command"></span>
              <span class="cursor"></span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </foreignObject>
</svg>
