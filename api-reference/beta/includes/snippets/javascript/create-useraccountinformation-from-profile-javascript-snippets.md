---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 609c833dfddade2487f62ab90aaf76c810e87dc2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441005"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userAccountInformation = {
  allowedAudiences: "organization",
  countryCode: "NO",
};

let res = await client.api('/me/profile/account')
    .version('beta')
    .post(userAccountInformation);

```