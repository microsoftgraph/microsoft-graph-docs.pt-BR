---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 702dbc2ae933f4e5e402135acd1d6d0f17061a583b1d97d807ab6fc2ad349b39
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/planner/rosters/6519868f-868f-6519-8f86-19658f861965/members')
    .version('beta')
    .get();

```