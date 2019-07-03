---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e09b7740e60fd71fd9adf6c9c2fd7f3498af3820
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519035"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}')
    .version('beta')
    .get();

```