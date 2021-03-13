---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f33b221af802a6c52ed2e0bed974887457c6b2d4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787177"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{id}/jobs/{id}/documents/{id}/uploadData')
    .version('beta')
    .post();

```