---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 80740bfbe0ea9e1f910a2b93fa151a04596bc54e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793837"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let supportedLanguages = await client.api('/me/outlook/supportedLanguages')
    .version('beta')
    .get();

```