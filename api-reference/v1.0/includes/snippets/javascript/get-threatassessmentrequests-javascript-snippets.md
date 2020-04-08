---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8411549a59b2d47e4aaaba0a8572088af100ecb3
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "42815951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/informationProtection/threatAssessmentRequests')
    .get();

```