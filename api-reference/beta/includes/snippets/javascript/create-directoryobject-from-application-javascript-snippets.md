---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 949594b6358985c3614aeea0bea3309ca55c8e787b4ba43612feba85461c7500
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100101"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
'@odata.id': 'https://graph.microsoft.com/beta/directoryObjects/{id}'
};

await client.api('/applications/{id}/owners/$ref')
    .version('beta')
    .post(directoryObject);

```