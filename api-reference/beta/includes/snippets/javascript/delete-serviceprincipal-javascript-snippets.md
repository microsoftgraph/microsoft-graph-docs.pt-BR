---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8daf93612223aaee9cc0e26c1c6b5a660924f588
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717837"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}')
    .version('beta')
    .delete();

```