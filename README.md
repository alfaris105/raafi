<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WhatsApp Bug Hunter 🕵️‍♂️</title>
    <link rel="stylesheet" href="style.css">
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/feather-icons/dist/feather.min.js"></script>
    <script src="https://unpkg.com/feather-icons"></script>
    <script src="components/navbar.js"></script>
    <script src="components/footer.js"></script>
</head>
<body class="bg-gray-100 min-h-screen flex flex-col">
    <custom-navbar></custom-navbar>

    <main class="flex-grow container mx-auto px-4 py-8">
        <div class="max-w-4xl mx-auto bg-white rounded-xl shadow-md overflow-hidden p-6">
            <div class="text-center mb-8">
                <h1 class="text-3xl font-bold text-gray-800 mb-2">WhatsApp Bug Hunter 🕵️‍♂️</h1>
                <p class="text-gray-600">Discover and report WhatsApp vulnerabilities responsibly</p>
            </div>

            <div class="grid md:grid-cols-2 gap-6 mb-8">
                <div class="bg-green-50 p-6 rounded-lg border border-green-100">
                    <div class="flex items-center mb-4">
                        <i data-feather="alert-triangle" class="text-green-600 mr-3"></i>
                        <h2 class="text-xl font-semibold text-gray-800">Common WhatsApp Bugs</h2>
                    </div>
                    <ul class="space-y-2 text-gray-700">
                        <li class="flex items-start">
                            <i data-feather="chevron-right" class="text-green-500 mr-2 mt-1"></i>
                            <span>Message spoofing vulnerabilities</span>
                        </li>
                        <li class="flex items-start">
                            <i data-feather="chevron-right" class="text-green-500 mr-2 mt-1"></i>
                            <span>Media auto-download exploits</span>
                        </li>
                        <li class="flex items-start">
                            <i data-feather="chevron-right" class="text-green-500 mr-2 mt-1"></i>
                            <span>Group chat manipulation bugs</span>
                        </li>
                        <li class="flex items-start">
                            <i data-feather="chevron-right" class="text-green-500 mr-2 mt-1"></i>
                            <span>Status view tracking issues</span>
                        </li>
                    </ul>
                </div>

                <div class="bg-blue-50 p-6 rounded-lg border border-blue-100">
                    <div class="flex items-center mb-4">
                        <i data-feather="shield" class="text-blue-600 mr-3"></i>
                        <h2 class="text-xl font-semibold text-gray-800">Responsible Disclosure</h2>
                    </div>
                    <p class="text-gray-700 mb-4">Found a WhatsApp bug? Follow these steps:</p>
                    <ol class="space-y-2 text-gray-700 list-decimal list-inside">
                        <li>Document the vulnerability with screenshots/videos</li>
                        <li>Create a detailed reproduction steps</li>
                        <li>Submit to WhatsApp Security Team</li>
                        <li>Wait for acknowledgment before public disclosure</li>
                    </ol>
                </div>
            </div>

            <div class="bg-yellow-50 border border-yellow-100 rounded-lg p-6 mb-8">
                <div class="flex items-center mb-4">
                    <i data-feather="alert-circle" class="text-yellow-600 mr-3"></i>
                    <h2 class="text-xl font-semibold text-gray-800">Important Notice</h2>
                </div>
                <p class="text-gray-700">
                    This website is for educational purposes only. Unauthorized access to WhatsApp accounts or systems is illegal. 
                    Always follow ethical hacking guidelines and obtain proper permissions before testing.
                </p>
            </div>

            <div class="bg-white border border-gray-200 rounded-lg p-6">
                <h2 class="text-xl font-semibold text-gray-800 mb-4">Submit Bug Report</h2>
                <form class="space-y-4">
                    <div>
                        <label for="name" class="block text-sm font-medium text-gray-700 mb-1">Your Name</label>
                        <input type="text" id="name" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-2 focus:ring-green-500 focus:border-transparent">
                    </div>
                    <div>
                        <label for="email" class="block text-sm font-medium text-gray-700 mb-1">Email</label>
                        <input type="email" id="email" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-2 focus:ring-green-500 focus:border-transparent">
                    </div>
                    <div>
                        <label for="bug" class="block text-sm font-medium text-gray-700 mb-1">Bug Description</label>
                        <textarea id="bug" rows="4" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-2 focus:ring-green-500 focus:border-transparent"></textarea>
                    </div>
                    <div>
                        <label for="steps" class="block text-sm font-medium text-gray-700 mb-1">Reproduction Steps</label>
                        <textarea id="steps" rows="4" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-2 focus:ring-green-500 focus:border-transparent"></textarea>
                    </div>
                    <button type="submit" class="bg-green-600 hover:bg-green-700 text-white font-medium py-2 px-6 rounded-md transition duration-300 flex items-center">
                        <i data-feather="send" class="mr-2"></i> Submit Report
                    </button>
                </form>
            </div>
        </div>
    </main>

    <custom-footer></custom-footer>

    <script>
        feather.replace();
    </script>
    <script src="script.js"></script>
</body>
</html>
