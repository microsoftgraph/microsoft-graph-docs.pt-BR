---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4175a2a616e708ca6e4f258bb8a72a1b9a8769c9
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944727"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets')
    .get();

```