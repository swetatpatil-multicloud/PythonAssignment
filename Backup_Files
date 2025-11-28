import os
import sys
import shutil
import time

def backup_files(source, destination):
    # Loop through files in source folder
    for file in os.listdir(source):
        src = os.path.join(source, file)
        dst = os.path.join(destination, file)

        # Only copy files (skip folders)
        if os.path.isfile(src):
            # If file already exists, add timestamp
            if os.path.exists(dst):
                timestamp = time.strftime("%Y%m%d%H%M%S")
                name, ext = os.path.splitext(file)
                dst = os.path.join(destination, f"{name}_{timestamp}{ext}")

            shutil.copy(src, dst)
            print(f"Copied: {file}")

if __name__ == "__main__":
    # Expect source and destination from command line
    if len(sys.argv) == 3:
        backup_files(sys.argv[1], sys.argv[2])
    else:
        print("Usage: python backup.py <source_folder> <destination_folder>")
