```

const workerBlob = new Blob(
	[ '(', pdfjsWorkerFunction.toString(), ')()' ],
	{ type: 'application/javascript' },
);
const blobUrl = URL.createObjectURL(blob);

```