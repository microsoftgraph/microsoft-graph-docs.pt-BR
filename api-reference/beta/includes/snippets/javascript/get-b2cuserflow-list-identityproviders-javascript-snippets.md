---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 14c54c2243e4c00dc1271ba5981ce7ea7a784000cb618c3189481f4132f9dc69
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identity/b2cUserFlows/{id}/identityProviders')
    .version('beta')
    .get();

```