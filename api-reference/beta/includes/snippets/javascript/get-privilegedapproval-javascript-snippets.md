---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16d41d07c3bc4a3b8b594326b69de70a2c910a6f
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945255"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedApproval/{id}')
    .version('beta')
    .get();

```