---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd0fd05391305d9c2cc371a067bef88e9924a4e5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805445"
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