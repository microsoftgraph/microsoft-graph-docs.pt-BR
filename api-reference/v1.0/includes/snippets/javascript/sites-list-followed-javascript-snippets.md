---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 574a8dcac3c79a82ac905eb79643505facfec3fb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797849"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let followedSites = await client.api('/me/followedSites')
    .get();

```