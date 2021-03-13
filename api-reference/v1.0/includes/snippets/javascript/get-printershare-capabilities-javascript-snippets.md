---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 874a4576d8c57718dcdbb6390f20aad9110ee407
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771628"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printerShare = await client.api('/print/shares/{printerShareId}')
    .select('id,displayName,capabilities')
    .get();

```