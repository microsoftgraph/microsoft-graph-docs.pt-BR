---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 167363525ceab208e6c186db94b12a422e12e3a4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791026"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let event = await client.api('/me/events/AAMkADAGAADDdm4NAAA=/')
    .version('beta')
    .select('subject,body,bodyPreview,organizer,attendees,start,end,location,locations')
    .get();

```