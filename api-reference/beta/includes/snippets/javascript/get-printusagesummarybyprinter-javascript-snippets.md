---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 716d67a29201ee34abab7c0cf30bb8df84c6423b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441453"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/reports/dailyPrintUsageSummariesByPrinter/{id}')
    .version('beta')
    .get();

```