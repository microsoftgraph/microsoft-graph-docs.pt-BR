---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0ccb87e382ce90ff805d8990c097099e8331755e4ca1bade4f7c052c4097bac8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273334"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemEmail = {
  displayName: 'Business Email',
  type: 'work'
};

await client.api('/users/{userId}/profile/emails/{id}')
    .version('beta')
    .update(itemEmail);

```