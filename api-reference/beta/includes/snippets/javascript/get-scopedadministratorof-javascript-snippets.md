---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8822813e45580afdf98847645b3f8de4dd7ab38a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793952"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedRoleMemberOf = await client.api('/me/scopedRoleMemberOf')
    .version('beta')
    .get();

```