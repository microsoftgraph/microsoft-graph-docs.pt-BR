---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43b05913e067ad74e71c481a4e17fdd9aa3ed382171b7eeebced0ad4c639139e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159664"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  destinationId: 'deleteditems'
};

await client.api('/me/messages/AAMkADhAAATs28OAAA=/move')
    .version('beta')
    .post(message);

```