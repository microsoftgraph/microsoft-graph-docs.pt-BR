---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd0fd05391305d9c2cc371a067bef88e9924a4e5
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226676"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/me/getMemberGroups')
    .version('beta')
    .post(string);

```