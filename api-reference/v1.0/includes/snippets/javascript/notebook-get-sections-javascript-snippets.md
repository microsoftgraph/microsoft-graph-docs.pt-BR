---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1292dab511ef1bbdb71d061225fc429f1b2d2e62
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789184"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sections = await client.api('/me/onenote/notebooks/{id}/sections')
    .get();

```