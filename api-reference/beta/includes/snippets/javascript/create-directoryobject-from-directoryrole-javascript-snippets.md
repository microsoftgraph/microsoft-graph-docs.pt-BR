---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 867146d91976e1beba55eb7bfd00924c7b0c426e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  directoryObject: {
  }
};

let res = await client.api('/directoryRoles/{id}/members/$ref')
    .version('beta')
    .post({directoryObject : directoryObject});

```