---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 084c157643c4adb9626af746e1edb368d1716e69
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getPrinterArchivedPrintJobs = await client.api('/print/reports/getPrinterArchivedPrintJobs(printerId='016b5565-3bbf-4067-b9ff-4d68167eb1a6',startDateTime=2021-05-24,endDateTime=2021-05-25)')
    .version('beta')
    .get();

```