---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4785fc0d11825b0311d4a34cfabdd495b1d509b6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468502"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailActivityCounts(period='D7')')
    .get();

```