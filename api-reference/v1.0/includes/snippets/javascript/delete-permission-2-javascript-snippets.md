---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 894839764468ff5b25ff7b8f9cd2e53bc0c49650
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952704"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .delete();

```