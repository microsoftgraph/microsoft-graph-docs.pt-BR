---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48154e70c2aef726068d740131ea7093fddee78e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479186"
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
    .update({inferenceClassificationOverride : inferenceClassificationOverride});

```