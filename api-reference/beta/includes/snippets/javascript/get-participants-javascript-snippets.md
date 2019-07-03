---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a523035e3b4778a6529fb35a785c3579d4c4ec54
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants')
    .version('beta')
    .header('Authorization','Bearer <TOKEN>')
    .get();

```