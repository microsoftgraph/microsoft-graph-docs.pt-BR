---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a070ba79e8377f3ae7a553d5c63f8c1aea922ac6
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240980"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewPolicy = await client.api('/policies/accessReviewPolicy')
    .version('beta')
    .get();

```