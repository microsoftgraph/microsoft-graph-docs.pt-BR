---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 198906a89afbac1799066e84075482fe7253ad052fab4e8f089d11c4726273ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329415"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/identityProviders/{id}')
    .delete();

```