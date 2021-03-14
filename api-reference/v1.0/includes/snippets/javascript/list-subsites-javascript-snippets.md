---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5ec57a406712b3afb4f22edcb88ac04e17c06d1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803420"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sites = await client.api('/sites/{site-id}/sites')
    .get();

```