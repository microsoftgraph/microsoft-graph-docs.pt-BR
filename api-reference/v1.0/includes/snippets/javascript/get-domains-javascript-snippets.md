---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61e8a3fe7f057b300c5ba6f0f49ec396b07400ca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798999"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let domains = await client.api('/domains')
    .get();

```