---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e888220f05ad545d2b31f5eff86de55cee49445b7ef522e561654ca76b3a2676
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099715"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/owners/{id}/$ref')
    .version('beta')
    .delete();

```