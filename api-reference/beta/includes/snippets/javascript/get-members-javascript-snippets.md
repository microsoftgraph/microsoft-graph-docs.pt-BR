---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29992c62d99137b67db52825953372417bade8db
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705643"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11016/members')
    .version('beta')
    .get();

```