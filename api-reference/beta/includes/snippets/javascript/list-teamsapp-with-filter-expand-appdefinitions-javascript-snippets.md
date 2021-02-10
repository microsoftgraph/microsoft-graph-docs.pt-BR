---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d94e238497c54719859fbb310084c986e17b9a2c
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('id eq '876df28f-2e78-423b-94a5-44181bd0e225'')
    .expand('appDefinitions')
    .get();

```