---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9f058ae82901431230f319bbc359c5c2804e269afe2c2b923cf226a527bb77e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327863"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarView = await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-10-01T19:00:00.00-08:00')
    .version('beta')
    .header('Prefer','outlook.body-content-type="text"')
    .get();

```