---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0971414ad06be27817163450addb00f514ac1b69
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799193"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sections = await client.api('/me/onenote/sections')
    .get();

```