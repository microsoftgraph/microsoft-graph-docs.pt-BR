---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2acb3d3fe202255ff568435a3ab0da732b7aac1c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803996"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/calendar')
    .version('beta')
    .delete();

```