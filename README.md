An M.2 A+E to mPCIe adapter for coral TPU

The capacitors most likely do not need to be populated

mPCIe Connector: [TE Connectivity 1775862-2](https://www.digikey.co.uk/en/products/detail/te-connectivity-amp-connectors/1775862-2/5430585)  
Standoffs: [Würth Elektronik 9774027151R](https://www.digikey.co.uk/en/products/detail/w%C3%BCrth-elektronik/9774027151R/5320625)  
  
Make sure to disable ASPM to prevent the coral from sleeping and not being able to wake  
Edit `/etc/default/grub`  
Example:  
`GRUB_CMDLINE_LINUX_DEFAULT="quiet intel_iommu=on pcie_aspm=off`

<p float="left">
  <img src="/images/board.PNG" width="30%" />
  <img src="/images/3d.PNG" width="30%" /> 
  <img src="/images/3dcoral.PNG" width="30%" />
</p>
