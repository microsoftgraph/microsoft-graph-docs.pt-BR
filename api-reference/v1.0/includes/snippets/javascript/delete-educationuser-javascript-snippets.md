---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ed636ed837fe82a29eafb892b36174d1b415f93634ec3646b1a5704cc1db850
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275163"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/users/{user-id}')
    .delete();

```