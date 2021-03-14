---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e693aa2acda9d466368ecf12b5014422fe177a1e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let event = await client.api('/me/events/AAMkADAGAADDdm4NAAA=')
    .select('subject,body,bodyPreview,organizer,attendees,start,end,location,locations')
    .get();

```