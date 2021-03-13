---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4b6627241b41159e935d200da64aa932fd0e15a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roomlist = await client.api('/places/microsoft.graph.roomlist')
    .version('beta')
    .get();

```