---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9863db4e3c60bd7aaa90679e2bae7ebe6bc05ab
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsDeviceUsageUserDetail(period='D7')')
    .version('beta')
    .get();

```