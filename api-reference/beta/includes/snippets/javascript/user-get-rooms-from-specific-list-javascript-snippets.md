---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 07798bf2ea25e036430f6a4e22edbc203ed91ffe
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615739"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com')')
    .version('beta')
    .get();

```