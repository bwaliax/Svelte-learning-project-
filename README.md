import 'svelte/internal/disclose-version';
import * as $ from 'svelte/internal/client';

var root = $.template(`<main class="svelte-5a4g00"><h1 class="svelte-5a4g00"></h1> <p class="svelte-5a4g00"></p> <p class="svelte-5a4g00"></p> <label for="nameInput">Want to personalize it?</label> <input id="nameInput" placeholder="Type your name..." class="svelte-5a4g00"></main> <h1 class="svelte-5a4g00"></h1>`, 1);

export default function App($$anchor) {
	let name = "Wecisankonde"; // Personalized name
	let message = "You are strong, capable, and loved. Keep shining your light!";
	let from = "Love of Your Life"; // Who it's from
	var fragment = root();
	var main = $.first_child(fragment);
	var h1 = $.child(main);

	h1.textContent = `Hello ${name ?? ''}!`;

	var p = $.sibling(h1, 2);

	p.textContent = message;

	var p_1 = $.sibling(p, 2);
