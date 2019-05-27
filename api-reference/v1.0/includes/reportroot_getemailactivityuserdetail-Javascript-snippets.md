---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44e4c2978e315b03a05e01ab555079fbb0e5eeca
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468483"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailActivityUserDetail(period='D7')')
    .get();

```