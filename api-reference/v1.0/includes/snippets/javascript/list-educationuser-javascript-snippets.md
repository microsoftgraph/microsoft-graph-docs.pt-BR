---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 205fc1f1e9dfa5bac7a194f212201e534855942a
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475372"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/education/users')
    .get();

```