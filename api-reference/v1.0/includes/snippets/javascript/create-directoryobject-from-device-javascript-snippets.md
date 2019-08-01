---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42065907c79dc236739bc60e80781173d06bad8b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715603"
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

let res = await client.api('/devices/{id}/registeredUsers')
    .post({directoryObject : directoryObject});

```