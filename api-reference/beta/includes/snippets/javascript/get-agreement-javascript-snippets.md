---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd0fcd02bf174e1058ae5be8f40f81dcef4a2191
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/agreements/'id'')
    .version('beta')
    .expand('files')
    .get();

```