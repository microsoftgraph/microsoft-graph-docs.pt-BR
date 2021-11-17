---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93f45a592c185a663fdb6fd1a09eff60ff4d28c650227b73de027b1ebfa8e2c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213638"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/extensionProperties/{id}')
    .version('beta')
    .delete();

```