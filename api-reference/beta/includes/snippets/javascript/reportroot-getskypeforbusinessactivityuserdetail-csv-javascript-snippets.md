---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce99740ccabce8c45740c1a9f663e384e0bca310
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726878"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessActivityUserDetail(period='D7')')
    .version('beta')
    .get();

```