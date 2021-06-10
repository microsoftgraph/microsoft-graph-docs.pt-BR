---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b55bb098f0a3ba0e9a47a76fb7601904e5b21945
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870084"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/roleManagement/cloudPC/roleAssignments/id')
    .version('beta')
    .delete();

```