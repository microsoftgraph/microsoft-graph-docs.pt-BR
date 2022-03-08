---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e38d9a75702542090eb3cd239d6b88b2900c52ae
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333509"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcSnapshot = await client.api('/deviceManagement/virtualEndpoint/snapshots/A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8')
    .version('beta')
    .get();

```