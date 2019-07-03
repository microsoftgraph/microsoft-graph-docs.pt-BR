---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 14f229af2594a7092fa569871ba9cf1086b91adb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/special/{name}/children')
    .version('beta')
    .get();

```