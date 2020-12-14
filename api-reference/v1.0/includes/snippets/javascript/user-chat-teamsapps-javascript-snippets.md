---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0ef3a38c402a50655a50e06ecebf77f62d82f2d
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49656995"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/teamwork/installedApps/{id}/chat')
    .get();

```