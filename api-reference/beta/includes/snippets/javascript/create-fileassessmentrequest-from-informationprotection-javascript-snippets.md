---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 556ab7299743e5a2cac63d1472215ea7bcc68e0d
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "40871727"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const threatAssessmentRequest = {
  @odata.type: "#microsoft.graph.fileAssessmentRequest",
  expectedAssessment: "block",
  category: "malware",
  fileName: "test.txt",
  contentData: "VGhpcyBpcyBhIHRlc3QgZmlsZQ=="
};

let res = await client.api('/informationProtection/threatAssessmentRequests')
    .version('beta')
    .post(threatAssessmentRequest);

```