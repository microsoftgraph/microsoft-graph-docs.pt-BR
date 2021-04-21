---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 105cf05e6bc6f9a5b05996b5ae04dcaaf94b420a
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2xUserFlows = await client.api('/identity/b2xUserFlows')
    .expand('identityProviders')
    .get();

```