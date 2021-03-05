---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3d59fd9fb87fc2ccbec842f483ed36fa0c812924
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471025"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groups = await client.api('/groups')
    .version('beta')
    .filter('membershipRuleProcessingState eq \'On\'')
    .select('id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus')
    .get();

```