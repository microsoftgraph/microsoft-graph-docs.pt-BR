---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1c334d929bdc359c126bf7266644fa24c9959eb9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795118"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttributeAssignment = {
    isOptional: false,
    requiresVerification: false,
    userInputType: 'TextBox',
    displayName: 'Shoe size',
    userAttributeValues: [],
    userAttribute: {
        id: 'extension_guid_shoeSize'
    }
};

await client.api('/identity/b2cUserFlows/B2C_1_Consumer/userAttributeAssignments')
    .version('beta')
    .post(identityUserFlowAttributeAssignment);

```