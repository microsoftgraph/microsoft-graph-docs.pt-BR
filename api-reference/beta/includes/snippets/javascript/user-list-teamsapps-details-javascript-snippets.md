---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 90447507577c6cc80dc8e4b856d485b45a089392
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809857"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/users/{id}/teamwork/installedApps')
    .version('beta')
    .expand('teamsAppDefinition($expand=bot)')
    .get();

```