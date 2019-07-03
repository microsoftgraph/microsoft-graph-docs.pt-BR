---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a82aca3ed7ea3a424def1b86d09da02c916d96c6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477555"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/people')
    .version('beta')
    .get();

```