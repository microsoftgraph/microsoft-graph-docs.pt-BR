---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c14cb7c3c5666c3ad02df67a594ec8ed827909de89ae769d8460b8ac5df57db3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375927"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .get();

```