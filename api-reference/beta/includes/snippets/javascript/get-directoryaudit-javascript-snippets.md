---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f5be1b5195cfdd9fd07ec14232d9d664565a4d46
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605884"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/directoryAudits/{id}')
    .version('beta')
    .get();

```