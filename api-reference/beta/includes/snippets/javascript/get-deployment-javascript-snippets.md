---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 005af9e27972173ec10180a0485f940edbb8e308
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let deployment = await client.api('/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5')
    .version('beta')
    .get();

```