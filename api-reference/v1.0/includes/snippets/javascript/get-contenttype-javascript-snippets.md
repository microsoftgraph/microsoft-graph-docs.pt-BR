---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8936d5f86c57d3320bd777ff13229c35a4b2155e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147566"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contentType = await client.api('/sites/{site-id}/contentTypes/{contentType-id}')
    .get();

```