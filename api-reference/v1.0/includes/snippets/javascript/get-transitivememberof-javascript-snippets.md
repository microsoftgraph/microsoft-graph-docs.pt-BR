---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 936a25d4364bdba7f4fccd4f29a90e78f42f2563
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805953"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/users/{id}/transitiveMemberOf')
    .get();

```