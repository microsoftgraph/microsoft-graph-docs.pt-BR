---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15e8f1f739783669bb15b369c04aa017c61a8c2b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507486"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}')
    .get();

```