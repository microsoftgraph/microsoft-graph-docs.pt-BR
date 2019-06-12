---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9270b7997c17b1f1706bb36119eb28620f6a88ad
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34843679"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarView/delta')
    .header('Prefer','odata.maxpagesize=2')
    .skiptoken('R0usmcCM996atia_s')
    .get();

```