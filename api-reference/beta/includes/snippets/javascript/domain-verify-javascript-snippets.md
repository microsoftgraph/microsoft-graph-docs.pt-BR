---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2025e60866769f5c4f24f59b26eedd59e6f8d73d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795561"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/domains/contoso.com/verify')
    .version('beta')
    .post();

```