---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3a47c1fbe40b1159ea5271f2c24ea85803cac220f9d68362e02a3dac47ff557
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215454"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let findRooms = await client.api('/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com')')
    .version('beta')
    .get();

```