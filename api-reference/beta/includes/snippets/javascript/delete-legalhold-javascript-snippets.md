---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 593da263f594e0dfeed174c99260e94d2caadc87421db7d55197650b5015ebfa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375816"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}')
    .version('beta')
    .delete();

```