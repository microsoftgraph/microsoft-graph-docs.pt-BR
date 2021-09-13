---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42db2bf693a7a1a9068b67596655935986e3cfe2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59097831"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleDefinition = await client.api('/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c')
    .expand('inheritsPermissionsFrom')
    .get();

```