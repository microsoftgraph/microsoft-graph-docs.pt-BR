---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd1b7e1f747d097d952a205032797f30b7924692
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/identityProviders/{id}')
    .delete();

```