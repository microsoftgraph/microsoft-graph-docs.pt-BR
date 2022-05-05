---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbee682b28a34aa033f7ea491e2405207083b24a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let list = await client.api('/sites/{siteId}/lists/{listId}')
    .version('beta')
    .get();

```