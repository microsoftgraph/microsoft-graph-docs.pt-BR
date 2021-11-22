---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed8f943e8463b4068fceecd86522cbd71bfc140ff99b03e7e33ab6b8612203ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274909"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/oauth2PermissionGrants/delta')
    .version('beta')
    .get();

```