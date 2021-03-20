---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0527a1d9faaeaff4abd5dbbb3dc8f13719cddb8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let dailyPrintUsageSummariesByPrinter = await client.api('/print/reports/dailyPrintUsageSummariesByPrinter')
    .version('beta')
    .get();

```