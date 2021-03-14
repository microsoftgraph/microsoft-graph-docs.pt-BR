---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6afa757aa9e5d5f7838340d9b099ba0d88894952
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808817"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/education/classes/{class-id}/members')
    .get();

```