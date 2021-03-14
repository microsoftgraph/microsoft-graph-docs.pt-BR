---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff0020d330f8ae8d92ab40d8ab1e9dbecbc3943e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802341"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let call = await client.api('/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92')
    .get();

```