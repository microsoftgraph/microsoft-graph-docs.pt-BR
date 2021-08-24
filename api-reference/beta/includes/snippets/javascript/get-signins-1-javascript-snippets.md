---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4209f6d5290e87532508dd01adb38c7c49a341a73b1331c5bc5854386cfeca9f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIns = await client.api('/auditLogs/signIns')
    .version('beta')
    .get();

```