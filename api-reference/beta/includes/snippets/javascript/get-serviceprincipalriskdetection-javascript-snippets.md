---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e951d7ac577c5547be7b418304378cfa50aee79b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337282"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipalRiskDetection = await client.api('/identityProtection/servicePrincipalRiskDetections/{servicePrincipalRiskDetectionId}')
    .version('beta')
    .get();

```