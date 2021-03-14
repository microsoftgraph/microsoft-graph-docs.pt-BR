---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4ffdf120ac6b1990a252844502dc747d274c37c0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806441"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let masterCategories = await client.api('/me/outlook/masterCategories')
    .get();

```