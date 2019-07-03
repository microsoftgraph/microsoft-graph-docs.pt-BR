---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83f44945f15bf60c136df37742f2cc8d614c20d8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508123"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/registeredOwners')
    .get();

```