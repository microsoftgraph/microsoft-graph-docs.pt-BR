---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95c3e84a9972764b94c039fb9ec8724a5dd72d80
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779264"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/devices/{id}')
    .delete();

```