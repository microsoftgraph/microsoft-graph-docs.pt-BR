---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9dd33b3a064b6075a2afc0f8c038f9cac75350e3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946713"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/beta/directoryObjects/{id}'
};

await client.api('/devices/{id}/registeredUsers/$ref')
    .version('beta')
    .post(directoryObject);

```