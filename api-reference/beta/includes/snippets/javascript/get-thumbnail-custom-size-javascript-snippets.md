---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 439afbcfe19285f1ca067869608800d0770b3224
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61228316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let thumbnails = await client.api('/me/drive/items/{item-id}/thumbnails?select=c300x400_crop')
    .version('beta')
    .get();

```