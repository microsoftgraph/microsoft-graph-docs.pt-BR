---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a02dae90cedea6bcd211c4468dbe590c99dc38a2
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225623"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const customSecurityAttributeDefinition = {
  description: 'Target completion date (YYYY/MM/DD)',
};

await client.api('/directory/customSecurityAttributeDefinitions/Engineering_ProjectDate')
    .version('beta')
    .update(customSecurityAttributeDefinition);

```