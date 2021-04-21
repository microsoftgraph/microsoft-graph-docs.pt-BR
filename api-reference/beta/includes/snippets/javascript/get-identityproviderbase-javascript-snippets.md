---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35dc00c5749cf035599ba518c31b3af33f60d862
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921376"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identity/identityProviders')
    .version('beta')
    .get();

```