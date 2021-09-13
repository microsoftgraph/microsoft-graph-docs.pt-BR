---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba480ff97aeb6709c50c2a09ce0772635c5c0962c28c6eafbe8195eb96fef2f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102721"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryAudits = await client.api('/auditLogs/directoryAudits')
    .get();

```