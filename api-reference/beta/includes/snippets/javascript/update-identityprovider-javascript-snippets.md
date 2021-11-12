---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8452226424e0d5147cbf901a720ee786e862a06f206e97578aa598ef395b0eec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102304"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
  clientSecret: '1111111111111'
};

await client.api('/identityProviders/Amazon-OAuth')
    .version('beta')
    .update(identityProvider);

```