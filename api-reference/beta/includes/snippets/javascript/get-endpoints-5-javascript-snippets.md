---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d324d220bf790635722eb7a4ec64da1f8b78a2f6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954272"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let monthlyPrintUsageSummariesByPrinter = await client.api('/print/reports/monthlyPrintUsageSummariesByPrinter')
    .version('beta')
    .get();

```