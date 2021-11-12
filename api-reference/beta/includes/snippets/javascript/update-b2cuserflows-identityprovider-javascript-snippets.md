---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 452912c03bd5f9bcb2d823f2f22039afff05b8671e2c33455e794994622b251c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157462"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
  '@odata.id': 'https://graph.microsoft.com/beta/identityProviders/{id}'
};

await client.api('/identity/b2cUserFlows/{id}/identityProviders/$ref')
    .version('beta')
    .post(identityProvider);

```