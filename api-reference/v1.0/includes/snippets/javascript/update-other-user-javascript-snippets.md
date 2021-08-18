---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67f9c71958e60b995a3480251e010fe968cd0c4ef97c571cbb4126ede7b13a8d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156855"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  businessPhones: [
    '+1 425 555 0109'
  ],
  officeLocation: '18/2111'
};

await client.api('/users/{id}')
    .update(user);

```