---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9b1b171f0e1b63969044ebce557bbf27353e82f0
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d')
    .delete();

```