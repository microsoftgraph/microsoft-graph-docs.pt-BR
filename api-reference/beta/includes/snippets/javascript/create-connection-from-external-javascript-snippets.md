---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9893e9a759eeef169480e7e3ce12e54c9598d4ee1c3fa1f7900878cfcd5e027
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157000"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalConnection = {
  id: 'contosohr',
  name: 'Contoso HR',
  description: 'Connection to index Contoso HR system'
};

await client.api('/external/connections')
    .version('beta')
    .post(externalConnection);

```