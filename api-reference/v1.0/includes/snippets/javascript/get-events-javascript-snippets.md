---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06d9b852625acab9ebb9766d16d687b569ffe15a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618256"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events')
    .header('Prefer','outlook.timezone="Pacific Standard Time"')
    .select('subject,body,bodyPreview,organizer,attendees,start,end,location')
    .get();

```