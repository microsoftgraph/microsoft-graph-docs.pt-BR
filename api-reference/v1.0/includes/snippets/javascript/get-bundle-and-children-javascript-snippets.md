---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db37ca72cabb05724d7b2f891b9c8bd8669e3010
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757961"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/drive/items/{bundle-id}?expand=children')
    .version('beta')
    .get();

```