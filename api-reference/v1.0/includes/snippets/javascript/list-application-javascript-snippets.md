---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7adb6a56561e4a9ce8dae628b1f388cd2f1ac79
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798555"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applications = await client.api('/applications')
    .get();

```