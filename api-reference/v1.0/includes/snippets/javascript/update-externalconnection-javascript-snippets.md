---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59df58e613871dc1e3db9545dd537ad92d47e9af
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687933"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalConnection = {
  name: 'Contoso HR Service Tickets',
  description: 'Connection to index HR service tickets'
};

await client.api('/external/connections/contosohr')
    .update(externalConnection);

```