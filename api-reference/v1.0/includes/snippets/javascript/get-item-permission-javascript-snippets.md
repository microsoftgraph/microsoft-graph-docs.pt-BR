---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dac5eb2f4f5139d96b9ad15e257260b966e09585
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/permissions/{perm-id}')
    .get();

```