---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc75c2ae8dc12eebd1c137d7a919ca7327869c74
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793465"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groups = await client.api('/groups')
    .get();

```