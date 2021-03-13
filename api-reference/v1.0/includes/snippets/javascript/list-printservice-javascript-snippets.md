---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 172ddbed38f38d319138f1c04ae31ec7e074c8c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777198"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let services = await client.api('/print/services')
    .get();

```