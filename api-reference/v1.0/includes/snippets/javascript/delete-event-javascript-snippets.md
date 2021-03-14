---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2993a6742caef76d311c524d2563c1dca4a82abf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785603"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}')
    .delete();

```