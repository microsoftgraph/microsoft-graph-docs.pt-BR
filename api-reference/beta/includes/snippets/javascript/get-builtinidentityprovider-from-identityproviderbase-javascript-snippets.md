---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57b9f622fadf7ffcf1dd78010acd8af86047aafc
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921466"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviderBase = await client.api('/identity/identityProviders/MSASignup-OAUTH')
    .version('beta')
    .get();

```