---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51bc86a97b9fc11e3e5dc14427d503abac3bdc68
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/reset')
    .version('beta')
    .post();

```