---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7de37cf681136144ac4f56ac31298211852a8407ee74867be00723b58644253
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217188"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}')
    .version('beta')
    .delete();

```