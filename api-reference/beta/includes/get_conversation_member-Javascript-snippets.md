---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5039c8e7e58a08a3da225119fdfe8135d7617806
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546553"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/chats/{id}/members')
    .version('beta')
    .get();

```