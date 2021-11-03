---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9bc66b01c18bfcff231d1365f2b5233cc0cf31879a1f57676f774a553a9e9bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272716"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{siteId}/contentTypes/{contentTypeId}/unpublish')
    .version('beta')
    .post();

```