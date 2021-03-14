---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: daa4f9057248ba689ee3f837bf5f30ea6176f618
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806179"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversationThread = await client.api('/groups/{id}/threads/{id}')
    .get();

```