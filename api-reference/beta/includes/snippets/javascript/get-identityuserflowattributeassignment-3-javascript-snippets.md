---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6af32d21e2c452a2e1e913f168bc34c5d618b1c713c1cf60f1e551e88c4e4ca1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityUserFlowAttributeAssignment = await client.api('/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}')
    .version('beta')
    .get();

```