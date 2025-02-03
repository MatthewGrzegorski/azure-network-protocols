
<p align="center">
  <img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
<p>
  Hello there! This comprehensive guide walks you through how to monitor and manage network traffic between Azure Virtual Machines using Network Security Groups (NSGs) and Wireshark. In this tutorial, you'll learn to set up your environment, capture and analyze network traffic, and fine-tune NSG rules to control the flow of data. Whether you're new to network security or looking to deepen your understanding, this guide provides clear, actionable steps to ensure nothing is overlooked.
</p>

<h2>Environments and Technologies Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machines/Compute)</li>
  <li>Remote Desktop</li>
  <li>Various Command-Line Tools</li>
  <li>Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)</li>
  <li>Wireshark (Protocol Analyzer)</li>
</ul>

<h2>Operating Systems Used</h2>
<ul>
  <li>Windows 10 (21H2)</li>
  <li>Ubuntu Server 20.04</li>
</ul>

<h2>High-Level Steps</h2>
<ul>
  <li>Provision Azure Virtual Machines and establish basic connectivity.</li>
  <li>Configure Network Security Groups (NSGs) to control inbound and outbound traffic.</li>
  <li>Capture network traffic using Wireshark for in-depth protocol analysis.</li>
  <li>Experiment with NSG rules and observe the resulting changes in traffic behavior.</li>
</ul>

<h2>Step-by-Step Guide: Inspecting Traffic and Experimenting with NSGs</h2>
<ol>
  <li>
    <strong>Provision and Configure Virtual Machines</strong>
    <ul>
      <li>
        Log into your Azure portal and create two virtual machines—one running Windows 10 and one running Ubuntu Server 20.04.
      </li>
      <li>
        Ensure both VMs reside in the same Virtual Network to allow direct communication.
      </li>
      <li>
        Enable Remote Desktop on Windows and SSH on Ubuntu for management purposes.
      </li>
    </ul>
  </li>
  <li>
    <strong>Configure Network Security Groups (NSGs)</strong>
    <ul>
      <li>
        Create NSGs and attach them to the network interfaces or subnets of your VMs.
      </li>
      <li>
        Define inbound and outbound rules to control traffic—for example, allowing SSH, RDP, HTTP/S, and ICMP while blocking unused ports.
      </li>
      <li>
        Document both default and custom rules for reference and troubleshooting.
      </li>
    </ul>
  </li>
  <li>
    <strong>Capture Network Traffic with Wireshark</strong>
    <ul>
      <li>
        Install Wireshark on a machine that has network access to your Azure VMs, or install it on one of the VMs if appropriate.
      </li>
      <li>
        Start capturing traffic while executing various network activities (e.g., ping, SSH login, HTTP requests) between the VMs.
      </li>
      <li>
        Analyze the capture to identify key protocols and understand the behavior of your network before and after applying NSG rules.
      </li>
    </ul>
  </li>
  <li>
    <strong>Experiment with NSG Rules and Analyze Impact</strong>
    <ul>
      <li>
        Modify NSG rules to simulate different security scenarios, such as temporarily blocking a specific port.
      </li>
      <li>
        Use Wireshark to capture and compare the network traffic before and after changes, noting any dropped packets or altered protocol behaviors.
      </li>
      <li>
        Record your observations to understand the impact of each rule and refine your NSG configuration for optimal performance and security.
      </li>
    </ul>
  </li>
  <li>
    <strong>Document Findings and Finalize Configuration</strong>
    <ul>
      <li>
        Compile your observations, including screenshots or logs from Wireshark, to create a comprehensive record of your experiments.
      </li>
      <li>
        Adjust NSG rules as necessary to strike the right balance between security and network functionality.
      </li>
      <li>
        Finalize your configuration, ensuring that all changes are well-documented and communicated to your team or stakeholders.
      </li>
    </ul>
  </li>
</ol>

<p>
  Thanks for following along! With these detailed steps, you're now equipped to effectively monitor and manage network traffic between your Azure VMs. This guide not only strengthens your network security through proper NSG configuration but also deepens your understanding of how various network protocols behave under different conditions. Happy monitoring, and here's to building a secure and efficient network environment!
</p>

</body>
</html>
