---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 082d33fe506f3640663f9d2cc74d346f8b640c12
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611943"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages')
    .top(2)
    .get();

```