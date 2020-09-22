---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b31a00722a35ba095c5ad05940de08af24854286
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027313"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/trustFramework/keySets/{id}/getActiveKey')
    .version('beta')
    .get();

```
