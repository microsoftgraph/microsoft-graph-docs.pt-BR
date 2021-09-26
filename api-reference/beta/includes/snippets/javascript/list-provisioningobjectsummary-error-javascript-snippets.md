---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3bd1818a00e9f1d7aca88e58d3a8829a94776b673c90c9be6814de8972c94ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159075"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let provisioning = await client.api('/auditLogs/provisioning')
    .version('beta')
    .get();

```