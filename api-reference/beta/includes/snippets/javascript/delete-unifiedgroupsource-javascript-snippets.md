---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb6705772d6ec29b9aa229a053cb3a790c86205b
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657142"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources/{unifiedGroupSourceId}')
    .version('beta')
    .delete();

```