---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12cb4232cd25f95950fbe5b16727a6d7ab4dc6ed
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038266"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{siteId}/contentTypes/{contentTypeId}/publish')
    .post();

```