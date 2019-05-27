---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a57c18985e8f5707d51d20493bdecff64b4227e9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479564"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/{school-id}')
    .get();

```