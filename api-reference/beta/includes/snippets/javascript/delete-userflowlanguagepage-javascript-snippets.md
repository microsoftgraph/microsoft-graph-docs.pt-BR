---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b63d5478179158b86b5b88cd46e9379f9c2d8b04
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844898"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages/phonefactor/$value')
    .version('beta')
    .delete();

```