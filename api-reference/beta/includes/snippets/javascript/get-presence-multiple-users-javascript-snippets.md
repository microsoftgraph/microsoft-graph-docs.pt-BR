---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57e6a11999a7cdb3e4143655f7632127c4082db0
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49846027"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const presence = {
  ids: ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
};

let res = await client.api('/communications/getPresencesByUserId')
    .version('beta')
    .post(presence);

```