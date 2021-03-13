---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1f82edb9814575825e3fb4671ba039ad80867d82
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let apiConnectors = await client.api('/identity/apiConnectors')
    .version('beta')
    .get();

```