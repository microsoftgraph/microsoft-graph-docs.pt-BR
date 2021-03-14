---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 614411879bff3f8ce7d0aa0e965dafaef875d4ec
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808086"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let registeredDevices = await client.api('/me/registeredDevices')
    .get();

```