---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8fca036dc159f791101ca3c5c1e2829ab105c3c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787859"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sharedWithMe = await client.api('/me/drive/sharedWithMe')
    .get();

```