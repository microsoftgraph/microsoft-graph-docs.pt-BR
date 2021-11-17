---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 094fc982f8a36bd033a9e8f14011b7dce8d0430e6f150a218db6f3f5b0f9fc36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}/dismissReminder')
    .version('beta')
    .post();

```