---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 308c9270f584c97176a4eb6b305a46590eb29f5a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive')
    .version('beta')
    .get();

```