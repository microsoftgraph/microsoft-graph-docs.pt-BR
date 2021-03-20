---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ebb1a95b4da90cfe05d6fb9b126cb67e1d04bbc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944512"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userAttributeAssignments = await client.api('/identity/b2xUserFlows/{id}/userAttributeAssignments')
    .version('beta')
    .get();

```