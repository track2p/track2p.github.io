# Suite2p-formatted output

---WORK IN PROGRESS---

In case the user selects the option `Save the outputs in suite2p format (containing cells tracked on all days)`, then re-indexed outputs are saved in a `matched_suite2p` folder, with the usual `stat.npy` and `F.npy` and others, just in a way that the first cell on one day corresponds to its match on the next. This is a user friendly format for custom downstream (already existing) analysis pipelines that rely on the suite2p format.