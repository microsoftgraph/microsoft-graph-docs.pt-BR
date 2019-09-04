---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bdcf3c42e0a7bffbd190d29920b06b263f12d321
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723361"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/provisioning')
    .version('beta')
    .get();

```