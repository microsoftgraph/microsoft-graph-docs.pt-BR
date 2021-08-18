---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9047375d83ae19df1c66bf2e052b357ff665e3c0c965c96b982b9fa82981216
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214865"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMembers = await client.api('/groups/{id}/transitiveMembers')
    .version('beta')
    .get();

```