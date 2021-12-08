---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 082d33fe506f3640663f9d2cc74d346f8b640c12
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336039"
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