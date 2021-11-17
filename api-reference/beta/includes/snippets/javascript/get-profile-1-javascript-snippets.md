---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb1623eaa48dc308077b29c0c94956f1bdce2a787d9069dfc70aa5e5f06cd2c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326869"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let profile = await client.api('/me/profile')
    .version('beta')
    .get();

```