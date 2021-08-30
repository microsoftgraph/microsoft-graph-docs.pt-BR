---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e312db42aca932d2b0800500d895f7628231c81a1f291f3a5a4e85fbbd9d293e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329655"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .filter('roleDefinitionId eq \'62e90394-69f5-4237-9190-012177145e10\'')
    .expand('principal')
    .get();

```