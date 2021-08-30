---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30c1c928c2cd98447476edc290b6e3c8936e4e100c4bfe07367cb2c18e3a8294
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156772"
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