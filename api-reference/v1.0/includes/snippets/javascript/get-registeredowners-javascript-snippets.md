---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4055b32f80121f8fed6fdd42a2d912577a94090e5b2fb111b8df43bf3fc728f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899527"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let registeredOwners = await client.api('/devices/{id}/registeredOwners')
    .get();

```