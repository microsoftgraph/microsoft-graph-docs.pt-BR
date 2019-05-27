---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0be9a5dbfb1a33a3561e1c615f3e7409f21a916
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469926"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/')
    .expand('itemattachment/item')
    .get();

```