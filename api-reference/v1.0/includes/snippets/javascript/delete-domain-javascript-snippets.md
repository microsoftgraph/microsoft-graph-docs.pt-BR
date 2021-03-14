---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6bdf3a902897eecf26b0a5eb2e91e739bbf9e00
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809477"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/domains/contoso.com')
    .delete();

```