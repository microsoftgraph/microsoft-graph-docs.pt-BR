---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2bd682fd2a29c3fae16fc8428b247f1f73d49339
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59016714"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let callRecord = await client.api('/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)')
    .get();

```