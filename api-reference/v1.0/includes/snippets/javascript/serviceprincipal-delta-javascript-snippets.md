---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 703223c433601becfa9239279d729dc5667cfb4b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/servicePrincipals/delta')
    .get();

```