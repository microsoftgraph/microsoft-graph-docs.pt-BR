---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f8547294388b0d3d8ff141e1da2fc6cf9a9d2c2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719598"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailAppUsageUserDetail(period='D7')')
    .version('beta')
    .get();

```