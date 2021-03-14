---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39051500f6c07a8e12207ac68485690a74df6856
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803681"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissions = await client.api('/sites/{sitesId}/permissions')
    .get();

```