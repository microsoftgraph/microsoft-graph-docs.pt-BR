---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f26d31cd970d2f782fec16513808d55c18a9d188
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let entries = await client.api('/admin/windows/updates/catalog/entries')
    .version('beta')
    .get();

```