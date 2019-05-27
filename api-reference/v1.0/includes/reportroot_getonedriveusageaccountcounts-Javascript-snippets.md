---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c958607343b85bfbecb889fdbad4cdada78c3fda
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435498"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageAccountCounts(period='D7')')
    .get();

```