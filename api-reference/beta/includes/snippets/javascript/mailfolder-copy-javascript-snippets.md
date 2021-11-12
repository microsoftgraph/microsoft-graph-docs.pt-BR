---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f62e95a42444f5a4a5fac1255f9afe2434976cbed1e9350567de8d6a22fbab45
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  destinationId: 'destinationId-value'
};

await client.api('/me/mailFolders/{id}/copy')
    .version('beta')
    .post(mailFolder);

```