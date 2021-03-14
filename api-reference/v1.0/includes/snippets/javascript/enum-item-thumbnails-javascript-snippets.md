---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1cd0a267c4b7b18b00016daf266d504c1580381
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780262"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let thumbnails = await client.api('/me/drive/items/{item-id}/thumbnails')
    .get();

```