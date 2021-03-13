---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06e8dc4528bd1a793689f6ed3f198234c92ea431
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkADYAAAImV_jAAA=/')
    .version('beta')
    .expand('eventMessage/event')
    .get();

```