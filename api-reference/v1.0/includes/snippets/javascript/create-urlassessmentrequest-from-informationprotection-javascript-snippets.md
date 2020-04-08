---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff77577394e5ff99f392f2a925abd936c7328c7d
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "42815841"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const threatAssessmentRequest = {
  @odata.type: "#microsoft.graph.urlAssessmentRequest",
  url: "http://test.com",
  expectedAssessment: "block",
  category: "phishing"
};

let res = await client.api('/informationProtection/threatAssessmentRequests')
    .post(threatAssessmentRequest);

```