---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3170dec4a712fea6a86eddd6d0f84a2dfc0ba6e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791028"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let overrides = await client.api('/me/inferenceClassification/overrides')
    .get();

```