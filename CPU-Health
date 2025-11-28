import psutil
import time

def monitor_cpu(threshold=80, interval=1):
    """
    Continuously monitor CPU usage.
    If usage exceeds threshold, display an alert.
    Runs until interrupted (Ctrl+C).
    """
    print("Monitoring CPU usage... Press Ctrl+C to stop.")
    try:
        while True:
            # Get CPU usage percentage
            cpu_usage = psutil.cpu_percent(interval=interval)
            
            # Print usage
            print(f"Current CPU usage: {cpu_usage}%")
            
            # Check against threshold
            if cpu_usage > threshold:
                print(f"⚠️ Alert! CPU usage exceeds threshold: {cpu_usage}%")
            
            # Sleep for interval (already handled by psutil, but safe to keep)
            time.sleep(interval)
    
    except KeyboardInterrupt:
        print("\nMonitoring stopped by user.")
    except Exception as e:
        print(f"❌ Error occurred: {e}")

# --- Main Program ---
if __name__ == "__main__":
    monitor_cpu(threshold=80, interval=1)
