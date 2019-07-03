---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8141bebcf8ef89c3a33cb6aa5026ede1844fe2fa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519505"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityDetail(period='D7')')
    .version('beta')
    .get();

```