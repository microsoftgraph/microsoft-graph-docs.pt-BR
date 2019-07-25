---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0363adf0e351f521aed0e0e447d91cc2826e1b2c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: "Volunteer"
};

let res = await client.api('/me/calendars')
    .version('beta')
    .post({calendar : calendar});

```