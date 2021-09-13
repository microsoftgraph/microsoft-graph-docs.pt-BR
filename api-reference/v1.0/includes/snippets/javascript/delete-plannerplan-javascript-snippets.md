---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c97e4f3ea5321d15ff8a0f86abe9ab4319e43771ab6706c6ec67f4c57f9a48a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899512"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/plans/{id}')
    .delete();

```