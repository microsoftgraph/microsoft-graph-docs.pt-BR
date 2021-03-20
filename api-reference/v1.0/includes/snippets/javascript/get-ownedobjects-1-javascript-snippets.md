---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acc19fcb666882d2f96a01fe2c4a1f2dd063079f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943416"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ownedObjects = await client.api('/servicePrincipals/{id}/ownedObjects')
    .get();

```