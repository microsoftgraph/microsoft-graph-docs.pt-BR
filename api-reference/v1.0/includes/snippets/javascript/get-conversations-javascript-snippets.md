---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a34c9925ceeb2334a3096d160c88d28c9ff39d9f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778431"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversations = await client.api('/groups/{id}/conversations')
    .get();

```