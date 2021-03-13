---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1504666924a987775e28324b0323aac17f0f5d90
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789273"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/todo/lists/AAMkADIyAAAhrbPXAAA=')
    .version('beta')
    .delete();

```