<script>
	import AuthInput from "@components/auth/AuthInput.svelte"
</script>

<form action="/api/auth/signin"
	  class="flex flex-col gap-2" method="POST"
>
	<AuthInput label="Email" type="email">
		<svg class="w-4 h-4 opacity-70" fill="currentColor" viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg">
			<path
				d="M2.5 3A1.5 1.5 0 0 0 1 4.5v.793c.026.009.051.02.076.032L7.674 8.51c.206.1.446.1.652 0l6.598-3.185A.755.755 0 0 1 15 5.293V4.5A1.5 1.5 0 0 0 13.5 3h-11Z" />
			<path
				d="M15 6.954 8.978 9.86a2.25 2.25 0 0 1-1.956 0L1 6.954V11.5A1.5 1.5 0 0 0 2.5 13h11a1.5 1.5 0 0 0 1.5-1.5V6.954Z" />
		</svg>
	</AuthInput>
	<AuthInput label="Password" type="password">
		<svg class="w-4 h-4 opacity-70" fill="currentColor" viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg">
			<path clip-rule="evenodd"
				  d="M14 6a4 4 0 0 1-4.899 3.899l-1.955 1.955a.5.5 0 0 1-.353.146H5v1.5a.5.5 0 0 1-.5.5h-2a.5.5 0 0 1-.5-.5v-2.293a.5.5 0 0 1 .146-.353l3.955-3.955A4 4 0 1 1 14 6Zm-4-2a.75.75 0 0 0 0 1.5.5.5 0 0 1 .5.5.75.75 0 0 0 1.5 0 2 2 0 0 0-2-2Z"
				  fill-rule="evenodd" />
		</svg>
	</AuthInput>
	<div class="flex items-center justify-between mt-1">
		<label class="cursor-pointer label-text text-sm flex">
			<input class="checkbox" type="checkbox" />
			<span class="ml-2">
                Remember me
            </span>
		</label>
		<a class="text-sm text-blue-500" href="/">
			Forgot password?
		</a>
	</div>
	<div>
		<button class="btn btn-success w-full mt-1 dark:text-white brightness-90">
			Sign In
		</button>
		<div class="ml-0.5 mt-0.5">
			<span class="text-sm text-gray-500">Don't have an account?</span>
			<a class="text-sm text-blue-500" href="/signup">Sign Up</a>
		</div>
	</div>
</form>
