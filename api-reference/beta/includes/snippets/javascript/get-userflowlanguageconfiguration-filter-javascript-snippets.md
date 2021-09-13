---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cbefccc60812b7458eb9248d1858ad2dc86e4fdb886f0ef54622aa526083f918
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157474"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let languages = await client.api('/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages')
    .version('beta')
    .filter('isEnabled eq true')
    .get();

```