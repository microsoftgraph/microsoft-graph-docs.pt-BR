---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7df26e0895bc5f326c5ca7c2cbc27aaec68148d9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464917"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsageDetail(period='D7')')
    .version('beta')
    .get();

```