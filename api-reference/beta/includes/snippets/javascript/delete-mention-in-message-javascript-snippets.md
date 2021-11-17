---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0446f15e5849db084bb17aa72a4b99a5bdf52982581f1ce1804bf075f53f0a12
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159665"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/messages/{id}/mentions/{id}')
    .version('beta')
    .delete();

```