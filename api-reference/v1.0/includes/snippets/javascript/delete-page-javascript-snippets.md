---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78ed77e547db480e67369f2de5c0f7f4a3cd5fbe96be1b2966cf399e966c30f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273572"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/onenote/pages/{id}')
    .delete();

```