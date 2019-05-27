---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6364e0c00d034109ea463bab9212bd86bcd6539a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')')
    .version('beta')
    .get();

```