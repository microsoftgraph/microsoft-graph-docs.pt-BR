---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44e9ee486c03606040628220ecfe4854ec288f88
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867128"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/informationProtection/threatAssessmentRequests/723c35be-8b5a-47ae-29c0-08d76ddb7f5b')
    .version('beta')
    .get();

```