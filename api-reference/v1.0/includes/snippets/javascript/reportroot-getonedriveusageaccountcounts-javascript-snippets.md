---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c958607343b85bfbecb889fdbad4cdada78c3fda
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735774"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageAccountCounts(period='D7')')
    .get();

```