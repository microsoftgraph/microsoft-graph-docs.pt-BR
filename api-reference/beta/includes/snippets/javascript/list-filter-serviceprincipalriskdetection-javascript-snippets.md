---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b407f70f7f968edf871d516182077b0590f05730
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334811"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipalRiskDetections = await client.api('/identityProtection/servicePrincipalRiskDetections')
    .version('beta')
    .filter('riskEventType eq \'investigationsThreatIntelligence\' or riskLevel eq \'medium\'')
    .get();

```