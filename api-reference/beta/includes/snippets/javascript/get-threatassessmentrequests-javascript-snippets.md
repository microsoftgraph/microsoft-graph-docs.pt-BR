---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce6c203fa066b480c5319ad077f53a2d5d9b6f30
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871730"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/informationProtection/threatAssessmentRequests')
    .version('beta')
    .get();

```