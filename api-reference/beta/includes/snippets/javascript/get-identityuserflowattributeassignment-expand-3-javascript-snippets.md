---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 058a228cb1436f52f464dc967b17354b3a55c9ce478cab0dc73c56fa8e41861e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102623"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityUserFlowAttributeAssignment = await client.api('/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}')
    .version('beta')
    .expand('userAttribute')
    .get();

```