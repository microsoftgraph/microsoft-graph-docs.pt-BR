---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca2002bdb928ba3ee9acf859f9c32ff34b590a5e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797683"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let recent = await client.api('/me/drive/recent')
    .version('beta')
    .get();

```