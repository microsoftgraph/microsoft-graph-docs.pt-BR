---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4db0b446f264b04269b2f1d93a4ddd69b53ce47
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let allowedValue = await client.api('/directory/customSecurityAttributeDefinitions/Engineering_Project/allowedValues/Alpine')
    .version('beta')
    .get();

```