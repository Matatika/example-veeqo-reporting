# Veeqo and Reporting Example Project

This is a very simple to use example project that contains Matatika's tap-veeqo, but also contains a demo of how to run Jupyter Notebooks in a Meltano project, including how to schedule them using the Matatika Ext plugin.

---

## Prerequisites

**NB - Currently this project is only supported to work on Linux and MacOS**

1. Get Docker - [https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/)
1. `wkhtmltopdf` installed on your system - [wkhtmltopdf Downloads Page](https://wkhtmltopdf.org/downloads.html)

---

## Steps

1. Clone and start up the project:
   ```terminal
   git clone git@github.com:Matatika/veeqo-reporting.git
   cd veeqo-reporting
   meltano install
   meltano invoke matatika lab
   ```

1. Your web browser automatically opens [https://localhost:3443](https://localhost:3443)

1. You will now see the tasks screen. You can optionally set up your Veeqo pipeline by:
   - Clicking `LET'S GO` for the "Complete pipeline configuration" task OR:
   - Click `Go To Lab`, then the Pipelines page. Here you should see a pipeline called `Report Pipeline`

1. Run the `Report Pipeline` by clicking the Play button.

1. Once the `Report Pipeline` has finished running, open your Meltano project on your local system, open the `output` dir. Here you should see an `report.pdf` which is the output from the pipeline being run.

Congratulations, you have now have a Notebook that executes on a scheudle in Meltano, using the Matatika lab.

---

### Support

Join our community on the [Matatika Slack](https://join.slack.com/t/matatika/shared_invite/zt-19n1bfokx-F31DNitTpSxWCFO2aFlgxg) to get help and updates.

You can read more about Matatika and our Lab in our [Documentation](https://www.matatika.com/docs/).

