---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 339f50ee58ec5c3bb425889742e75f81afb92995
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805175"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/messages/{id}')
    .delete();

```