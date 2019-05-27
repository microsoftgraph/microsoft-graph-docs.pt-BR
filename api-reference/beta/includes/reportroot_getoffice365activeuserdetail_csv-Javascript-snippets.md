---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 744d52ee0740329f903d8feca9b4288ac8119135
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441609"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActiveUserDetail(period='D7')')
    .version('beta')
    .get();

```