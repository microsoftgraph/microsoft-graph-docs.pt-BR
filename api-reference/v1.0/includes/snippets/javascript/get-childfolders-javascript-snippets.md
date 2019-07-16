---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96dff4c3c89320bef9febde72aed0432a3504434
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738712"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/{id}/childFolders')
    .get();

```