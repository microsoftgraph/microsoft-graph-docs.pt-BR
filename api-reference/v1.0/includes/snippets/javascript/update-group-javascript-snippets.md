---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9475b9b309ec5019a30f37b4f627a92b5d464b96
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722568"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: "description-value",
  displayName: "displayName-value",
  groupTypes: [
    "groupTypes-value"
  ],
  mail: "mail-value",
  mailEnabled: true,
  mailNickname: "mailNickname-value"
};

let res = await client.api('/groups/{id}')
    .update({group : group});

```