---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa4dda468645cddb587eebeb61bef86d2b44aced
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223935"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const allowedValue = {
    isActive: 'false'
};

await client.api('/directory/customSecurityAttributeDefinitions/Engineering_Project/allowedValues/Alpine')
    .version('beta')
    .update(allowedValue);

```