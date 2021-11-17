---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd418538db70111053d10b0d1223ef1bde5bb746278c355c240fdef9415996a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/domains/contoso.com')
    .version('beta')
    .delete();

```