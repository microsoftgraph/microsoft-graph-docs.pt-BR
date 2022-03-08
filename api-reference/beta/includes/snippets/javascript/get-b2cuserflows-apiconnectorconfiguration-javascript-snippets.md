---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edeb114b49c7a4de28ff76fb36ce3f861b304ec6
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63332405"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlowApiConnectorConfiguration = await client.api('/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration')
    .version('beta')
    .expand('postFederationSignup,postAttributeCollection')
    .get();

```