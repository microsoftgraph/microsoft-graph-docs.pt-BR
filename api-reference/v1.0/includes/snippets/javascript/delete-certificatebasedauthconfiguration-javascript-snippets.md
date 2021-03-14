---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28b6a94382ae925e3e0ca780d4afe57458f58a2f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805865"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/organization/{id}/certificateBasedAuthConfiguration/{id}')
    .delete();

```