<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Emergency Contact Numbers</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background: #f9f9f9;
            color: #333;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 0;
            margin: 0;
            overflow: auto; /* Allow scrolling when needed */
        }

        .container {
            background: #ffffff;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
            width: 100%;
            max-width: 600px;
            min-height: 100vh; /* Ensure it fills the screen */
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            padding: 10px;
            overflow-y: auto; /* Allow scrolling inside the container */
        }

        .header {
            background: #d32f2f;
            color: #ffffff;
            text-align: center;
            padding: 8px;
            flex-shrink: 0;
        }

        .header h1 {
            font-size: 18px;
        }

        .header p {
            font-size: 11px;
        }

        .instruction {
            text-align: center;
            font-size: 11px;
            padding: 5px;
            color: #555;
        }

        .numbers {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 5px;
            flex-grow: 1;
            padding: 5px;
            overflow-y: auto; /* Allow scrolling if numbers exceed space */
        }

        .number {
            display: flex;
            align-items: center;
            background: #f4f4f4;
            padding: 8px;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            font-size: 12px;
            justify-content: start;
        }

        /* Ensure "Channel 4" spans full width on smaller screens */
        .channel-4 {
            grid-column: 1 / -1;
            justify-content: center;
        }

        .icon {
            width: 30px;
            height: 30px;
            background: #d32f2f;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            border-radius: 50%;
            font-size: 14px;
            margin-right: 8px;
        }

        .info {
            font-size: 13px;
        }

        .info a {
            text-decoration: none;
            color: #d32f2f;
            font-weight: bold;
        }

        .footer {
            text-align: center;
            padding: 8px;
            font-size: 11px;
            background: #d32f2f;
            color: white;
            flex-shrink: 0;
        }

        @media (max-width: 480px) {
            .header h1 {
                font-size: 16px;
            }

            .header p {
                font-size: 10px;
            }

            .instruction {
                font-size: 10px;
            }

            .number {
                font-size: 11px;
            }

            .icon {
                width: 25px;
                height: 25px;
                font-size: 12px;
            }

            .info {
                font-size: 12px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Emergency Contact Numbers</h1>
            <p>Ambulance | Fire | Rescue | Security</p>
        </div>

        <div class="instruction">
            <b>Click on the numbers below to call directly in case of an emergency.</b>
        </div>

        <div class="numbers">
            <div class="number">
                <div class="icon">☎️</div>
                <div class="info">
                    <a href="tel:0322091333">0322 091 333</a> - Landline/Mobile
                </div>
            </div>

            <div class="number">
                <div class="icon">📞</div>
                <div class="info">
                    <a href="tel:800">800</a> - AGAG Landline
                </div>
            </div>

            <div class="number">
                <div class="icon">📲</div>
                <div class="info">
                    <a href="tel:0800400002">0800 400 002</a> - Toll Free/Mobile
                </div>
            </div>

            <div class="number">
                <div class="icon">🔒</div>
                <div class="info">
                    <a href="tel:0556582933">0556 582 933</a> - Security
                </div>
            </div>

            <div class="number">
                <div class="icon">🔒</div>
                <div class="info">
                    <a href="tel:0322296756">0322 296 756</a> - Security
                </div>
            </div>

            <div class="number">
                <div class="icon">🔒</div>
                <div class="info">
                    <a href="tel:0322296755">0322 296 755</a> - Security
                </div>
            </div>

            <!-- Channel 4 spans full width -->
            <div class="number channel-4">
                <div class="icon">📡</div>
                <div class="info">
                    <b>Channel 4 - Two-Way Radio</b>
                </div>
            </div>
        </div>

        <div class="footer">
            <strong>SENIOR MANAGER - HUMAN RESOURCES</strong>
            <p>Please avoid prank calls. This service is for emergencies only.</p>
        </div>
    </div>
</body>
</html>
