---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 891adbbf60eabe70281787f2433fc556fdbe1a78
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2020
ms.locfileid: "41123074"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-10-01T19:00:00.00-08:00')
    .version('beta')
    .header('Prefer','outlook.body-content-type="text"')
    .get();

```