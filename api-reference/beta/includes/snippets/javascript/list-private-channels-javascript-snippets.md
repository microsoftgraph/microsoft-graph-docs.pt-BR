---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f308ef06c8865e24a9e4087cb3e1f459b6ad5e2fa8091c36447699708ce59524
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159818"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channels = await client.api('/teams/64c323f2-226a-4e64-8ba4-3e6e3f7b9330/channels')
    .version('beta')
    .filter('membershipType eq \'private\'')
    .get();

```