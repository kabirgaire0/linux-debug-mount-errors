# Mounting mannually
`sudo mount -t ntfs /dev/nvme0n1p1 /media/kabir0423/storage1`
  
# Try Mounting with udisksctl
`sudo blkid /dev/nvme0n1p1`

# Install ntfs-3g Package
```
sudo apt update
sudo apt install ntfs-3g
```

# Try Mounting Manually with ntfs-3g
`sudo mount -t ntfs-3g /dev/nvme0n1p1 /media/kabir0423/storage1`

# Check and Repair the NTFS Filesystem
`sudo ntfsfix /dev/nvme0n1p1`

# Check the Mount Point
`sudo mkdir -p /media/kabir0423/storage1`

# Check Disk Health
```
sudo apt install smartmontools
sudo smartctl -a /dev/nvme0n1
```

