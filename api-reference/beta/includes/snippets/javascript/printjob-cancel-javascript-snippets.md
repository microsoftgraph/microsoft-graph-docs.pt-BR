---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acbea491f2d5a445357a665b3dfb5cda0e623052
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/jobs/{id}/cancel')
    .version('beta')
    .post();

```