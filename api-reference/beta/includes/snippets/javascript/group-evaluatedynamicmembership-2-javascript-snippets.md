---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 012c4a664f61872191b40db94b81bc110d78e8e8bb61c306680debae89cee7dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375836"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const evaluateDynamicMembershipResult = {
  memberId: '319b41e8-d9e4-42f8-bdc9-741113f48b33',
  membershipRule: '(user.displayName -startsWith \"EndTestUser\")'
};

await client.api('/groups/evaluateDynamicMembership')
    .version('beta')
    .post(evaluateDynamicMembershipResult);

```