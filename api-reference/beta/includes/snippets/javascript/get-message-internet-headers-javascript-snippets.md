---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db863740b02cb03639947e8d12fb6db7ba49b0ff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkAGVmMDEz/')
    .version('beta')
    .select('internetMessageHeaders')
    .get();

```