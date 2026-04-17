# Vortex Telemetry Engine - Dashboard Proxy

This repository serves as the frontend proxy and routing mask for the **Vortex Telemetry Engine** dashboard.

## Architecture Justification

The primary visual interface for Vortex is built using **Streamlit** and hosted on Streamlit Community Cloud. However, Streamlit Cloud restricts the use of custom domains on its free tier. 

To maintain a professional, unified brand identity (`dashboard.shubhampawar.in`), this repository is deployed as a microservice on **Vercel**. It utilizes a fullscreen, borderless `iframe` to seamlessly proxy the Streamlit interface under the custom domain, automatically securing the connection with a Vercel-managed SSL/TLS certificate.

## Developer Context

*Note: This specific routing microservice is hosted on my secondary GitHub account.*

* **Main GitHub Profile:** [github.com/Shubhtistic](https://github.com/Shubhtistic)
* **Main Backend Repository:** [Vortex Telemetry Engine Repo](https://github.com/Shubhtistic/vortex-telemetry-engine)

## Links

* **Live Dashboard:** [https://dashboard.shubhampawar.in](https://dashboard.shubhampawar.in)

## Service Availability Notice

This entire microservice architecture is currently running on free-tier cloud resources. **If the live dashboard or backend API is unresponsive, it means I am temporarily utilizing my server allocations to build and deploy another project.** The backend EC2 engine is spun up and down dynamically as needed for active development and demonstrations.