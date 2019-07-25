---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22c427b03471710aa7285942df1742d55f8015b5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705565"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inferenceClassificationOverride = {
  classifyAs: "focused"
};

let res = await client.api('/me/inferenceClassification/overrides/{id}')
    .version('beta')
    .update({inferenceClassificationOverride : inferenceClassificationOverride});

```