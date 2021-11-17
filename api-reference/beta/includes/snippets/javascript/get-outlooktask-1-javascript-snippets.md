---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74d84c5cfd4992241e0bc85966d39cd628372218f823412d2bed186e241aac7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899661"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outlookTask = await client.api('/me/outlook/tasks/AAMkADA1MTrgAAA=')
    .version('beta')
    .get();

```