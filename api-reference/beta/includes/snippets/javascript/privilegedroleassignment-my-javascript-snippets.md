---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4667886f38f44e4176c96a1d040c82bf148050135edcf516ff284683cd6a759
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898007"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let my = await client.api('/privilegedRoleAssignments/my')
    .version('beta')
    .get();

```