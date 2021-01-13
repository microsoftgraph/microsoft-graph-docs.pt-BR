---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a478b882acd9860a01e1f371da3a11095d53cd4b
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843996"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
    @odata.id: "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
};

let res = await client.api('/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref')
    .version('beta')
    .put(identityApiConnector);

```