---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02da2f480bc33ca2d0bc66f35ebfd5ee06a924d8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621809"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkADAGAADDdm4NAAA=/')
    .version('beta')
    .select('subject,body,bodyPreview,organizer,attendees,start,end,location,locations')
    .get();

```