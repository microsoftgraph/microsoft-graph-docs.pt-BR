---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7974788ae70881a91d187bff9b6be22ba6e3f36b6349297c118fdb726c664a78
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899775"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let events = await client.api('/groups/{id}/events')
    .version('beta')
    .get();

```