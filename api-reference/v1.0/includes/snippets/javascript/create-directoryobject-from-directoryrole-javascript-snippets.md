---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: daa172e4dc18e6b9b12cfd178e912e7aecfd667d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733609"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
};

let res = await client.api('/directoryRoles/{id}/members/$ref')
    .post({directoryObject : directoryObject});

```