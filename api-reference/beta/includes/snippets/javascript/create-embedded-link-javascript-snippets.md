---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3543fc8f60316c94e9dba4bc25541d7d3e6e87de
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713148"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: "embed"
};

let res = await client.api('/me/drive/items/{item-id}/createLink')
    .version('beta')
    .post(permission);

```