---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3cd9fa5a2348d10ca8c2c7171fe66b05628abf5d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715696"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/subscriptions/{id}')
    .delete();

```