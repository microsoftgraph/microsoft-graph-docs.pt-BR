---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d88e4b150d94ee801eb01d4281977f5e41652891c5c458e0f69529bddc99112f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274914"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemEmail = await client.api('/users/{userId}/profile/emails/{id}')
    .version('beta')
    .get();

```