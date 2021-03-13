---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66c8392b078b134322ffb99b0aa98ef3b6e9bc25
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50769355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/communications/calls/{id}/participants/{id}')
    .version('beta')
    .delete();

```