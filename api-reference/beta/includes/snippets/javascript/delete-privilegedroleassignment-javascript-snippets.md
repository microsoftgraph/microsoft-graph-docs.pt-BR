---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da294422d4d8ba0ebdec68c859e92d49dadefa57242167bcc61ba4603d21ddb9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159197"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/privilegedRoleAssignments/{id}')
    .version('beta')
    .delete();

```