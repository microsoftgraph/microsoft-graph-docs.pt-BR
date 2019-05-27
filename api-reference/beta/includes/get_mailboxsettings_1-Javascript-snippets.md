---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1c50c164319b4b9a1e39f7dfeef2696fff2555d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449136"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailboxSettings')
    .version('beta')
    .get();

```