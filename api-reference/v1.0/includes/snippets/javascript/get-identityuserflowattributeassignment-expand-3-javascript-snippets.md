---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0b1bcbf5b9ae7ec50230f4d3250e2cf46a2cc39c0be0e24e0fff83e62e878bb2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376699"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityUserFlowAttributeAssignment = await client.api('/identity/b2xUserFlows/{id}/userAttributeAssignments/{id}')
    .expand('userAttribute')
    .get();

```