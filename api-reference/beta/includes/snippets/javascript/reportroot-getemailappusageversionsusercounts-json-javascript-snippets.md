---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 466218397e6490804ec2a32f7409f5143f7f0e90
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476011"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailAppUsageVersionsUserCounts(period='D7')')
    .version('beta')
    .get();

```