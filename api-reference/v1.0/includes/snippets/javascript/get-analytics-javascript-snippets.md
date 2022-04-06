---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0548bd00c81df870674ea784b7e0c7d6b8b0520c
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528048"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemActivityStat = await client.api('/drives/{drive-id}/items/{item-id}/analytics/allTime')
    .get();

```