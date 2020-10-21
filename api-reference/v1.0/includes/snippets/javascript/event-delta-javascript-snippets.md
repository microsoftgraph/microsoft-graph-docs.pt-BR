---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 373337d7a5b296ff89efe7c0f3f88f97714cac5b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608260"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarView/delta?startdatetime=%7Bstart_datetime%7D&enddatetime=%7Bend_datetime%7D')
    .get();

```