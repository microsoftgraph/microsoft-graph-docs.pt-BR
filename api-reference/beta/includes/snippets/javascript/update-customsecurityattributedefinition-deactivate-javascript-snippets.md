---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0fce3263a6164dff7400f2df88086b5e1ba049c
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const customSecurityAttributeDefinition = {
  status: 'Deprecated'
};

await client.api('/directory/customSecurityAttributeDefinitions/Engineering_Project')
    .version('beta')
    .update(customSecurityAttributeDefinition);

```