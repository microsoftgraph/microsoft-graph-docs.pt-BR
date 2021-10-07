---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c669b3d093c99d98b06a67d1a6026c2923fb86b5
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214477"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getAllMessages = await client.api('/users/0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5/chats/getAllMessages')
    .top(2)
    .get();

```