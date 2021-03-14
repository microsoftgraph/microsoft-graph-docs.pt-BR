---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc0cc71eee80eb47d12f51eef7665563509f853d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805722"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forceDelete = {
  disableUserAccounts: true
};

await client.api('/domains/{id}/forceDelete')
    .post(forceDelete);

```