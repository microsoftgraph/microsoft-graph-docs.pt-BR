---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9fe08affd9b65ce65f27d19cab3aec1b0c866c0
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let availableProviderTypes = await client.api('/identity/identityProviders/availableProviderTypes')
    .version('beta')
    .get();

```