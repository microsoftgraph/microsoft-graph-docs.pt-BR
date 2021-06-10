---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 740fec3eef9312050f2af0301893d7f0cfd84cf6
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871594"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let monthlyPrintUsageByUser = await client.api('/print/reports/monthlyPrintUsageByUser')
    .version('beta')
    .get();

```