---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 233fef5d4a81e7514d619bc0aead13bf6f380213
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436667"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarview/delta')
    .version('beta')
    .get();

```