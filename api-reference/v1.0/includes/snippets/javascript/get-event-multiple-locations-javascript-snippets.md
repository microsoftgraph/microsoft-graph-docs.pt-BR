---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47656df44abb3c939c52e5533a7c579b77bc199d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609604"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkADAGAADDdm4NAAA=')
    .select('subject,body,bodyPreview,organizer,attendees,start,end,location,locations')
    .get();

```