---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f05fb346042439030607306a02ff333bbd450ff70416d0cbe145b85dbfd0677e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217571"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages/phonefactor/$value')
    .version('beta')
    .delete();

```