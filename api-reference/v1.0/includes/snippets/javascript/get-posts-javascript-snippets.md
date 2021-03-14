---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 891236efdb83b0e4ed7df93d73893bb6316d7453
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let posts = await client.api('/groups/{id}/threads/{id}/posts')
    .get();

```