---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 125612d28dd6bc3230a925c0d531f50d6909986b
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844520"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/apiConnectors/{id}')
    .version('beta')
    .delete();

```