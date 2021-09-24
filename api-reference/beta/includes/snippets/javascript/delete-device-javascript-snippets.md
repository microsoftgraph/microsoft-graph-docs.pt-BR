---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf8102ab31d14f65409e45366b5f1a7976cfea152782fdb645698dc549207cb6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159689"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/devices/{id}')
    .version('beta')
    .delete();

```