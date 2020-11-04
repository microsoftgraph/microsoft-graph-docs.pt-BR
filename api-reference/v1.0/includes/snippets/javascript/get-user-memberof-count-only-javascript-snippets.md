---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81fb4f62695357c16e89baab42f62ecb001a0553
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905834"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/memberOf/$count')
    .header('ConsistencyLevel','eventual')
    .get();

```