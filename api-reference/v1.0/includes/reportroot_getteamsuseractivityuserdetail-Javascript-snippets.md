---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6054330bc86993cf5eb204342ae5b3e0aebd2adf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsUserActivityUserDetail(period='D7')')
    .get();

```