---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 099074925568b22da84040005f5fc67336d2c15a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721645"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/inbox/messagerules')
    .version('beta')
    .get();

```