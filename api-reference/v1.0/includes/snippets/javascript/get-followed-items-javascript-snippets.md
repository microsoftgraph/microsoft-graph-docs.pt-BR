---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afaded7c6a5b8e123edf395d2c4d085eb40b0add
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790451"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let following = await client.api('/me/drive/following')
    .get();

```