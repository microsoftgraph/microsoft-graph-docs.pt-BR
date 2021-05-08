---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eea6c7f2a57a3cefe0cc94b6f6d34ed42fca11fb
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254192"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationRubric = await client.api('/education/classes/{id}/assignments/{id}/rubric')
    .version('beta')
    .get();

```