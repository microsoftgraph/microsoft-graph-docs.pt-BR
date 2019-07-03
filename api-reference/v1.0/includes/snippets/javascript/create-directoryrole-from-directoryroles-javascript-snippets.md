---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8afbfcb8ddb7650b27badb4fab6589f9aa8cbefd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465471"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryRole = {
  roleTemplateId: "roleTemplateId-value"
};

let res = await client.api('/directoryRoles')
    .post({directoryRole : directoryRole});

```