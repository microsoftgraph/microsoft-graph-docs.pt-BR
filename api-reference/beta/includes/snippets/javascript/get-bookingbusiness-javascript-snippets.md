---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb1bd588386dbc1930c0c9e443f5849e5eb0dd8d1aa95bbabeac8170dea4b340
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157640"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingBusiness = await client.api('/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com')
    .version('beta')
    .get();

```