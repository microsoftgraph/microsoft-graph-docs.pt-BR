---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: addc6ad9d7ea88e43a0c3798983ffa8f25dba23b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/notebooks/{id}/sections')
    .get();

```