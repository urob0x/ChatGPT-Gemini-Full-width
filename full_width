// ==UserScript==
// @name        LLM Full Width - ChatGPT Fixed
// @namespace   Violentmonkey Scripts
// @match       https://chatgpt.com/*
// @match       https://gemini.google.com/*
// @grant       GM_addStyle
// @version     1.1
// @author      AI Collaborator
// @description Forza el ancho completo en ChatGPT (incluso con la nueva UI) y Gemini.
// ==/UserScript==

(function() {
    'use strict';

    const css = `
        /* --- CORRECCIÓN PARA CHATGPT --- */

        /* Selecciona los contenedores de los mensajes y la caja de entrada */
        div.mx-auto.flex-1,
        div.md\\:max-w-3xl,
        div.lg\\:max-w-\\[40rem\\],
        div.xl\\:max-w-\\[48rem\\],
        div.xl\\:max-w-3xl,
        .md\\:max-w-2xl,
        .lg\\:max-w-3xl,
        .xl\\:max-w-4xl,
        /* Selector universal para cualquier clase de 'max-width' de Tailwind en el chat */
        div[class*="max-w-"] {
            max-width: 96% !important;
            width: 96% !important;
        }

        /* Ajuste para que el texto aproveche el espacio */
        article div.text-base {
            max-width: 100% !important;
            width: 100% !important;
        }

        /* --- CORRECCIÓN PARA GEMINI (Mantenida) --- */
        .message-content,
        .chat-container,
        .conversation-container,
        main-content {
            max-width: 96% !important;
        }
    `;

    if (typeof GM_addStyle !== 'undefined') {
        GM_addStyle(css);
    } else {
        const style = document.createElement('style');
        style.textContent = css;
        document.head.append(style);
    }
})();
