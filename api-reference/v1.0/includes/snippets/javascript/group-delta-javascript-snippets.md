---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55e2775e64316c444b925bbddb6d937f6961b103
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808412"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/groups/delta')
    .get();

```