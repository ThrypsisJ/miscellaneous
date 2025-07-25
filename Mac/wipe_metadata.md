## Remove "._*" and ".DS_Store" files
find /Volumes/{volume_name} -name "._*" -delete 2>/dev/null
find /Volumes/{volume_name} -name ".DS_Store" -delete 2>/dev/null
