---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 797801c29f9fd795823bf553717e934e17aeea8f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781824"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/removeFavorite')
    .post();

```