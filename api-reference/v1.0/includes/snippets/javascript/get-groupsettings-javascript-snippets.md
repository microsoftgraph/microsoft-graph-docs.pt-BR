---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b389c27441502a3377ff5d26d343f39b0e49d838
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466231"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupSettings')
    .get();

```