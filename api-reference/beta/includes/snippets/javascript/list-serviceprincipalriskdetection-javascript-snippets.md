---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88299d59dac58b12907b8d0c1dcb062daec31c6a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334832"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipalRiskDetections = await client.api('/identityProtection/servicePrincipalRiskDetections')
    .version('beta')
    .get();

```