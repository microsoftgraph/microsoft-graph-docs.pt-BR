---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 003cdf9140ad90cfd3392fd77fed4588b17dfe52
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "61030355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversation = await client.api('/groups/4d81ce71-486c-41e9-afc5-e41bf2d0722a/conversations/AAQkAGRhZmRhMWM3LTYwZTktNDZmYy1hNWU1LThhZWU4NzI2YTEyZgAQABKPPJ682apIiV1UFlj7XxY=')
    .version('beta')
    .get();

```