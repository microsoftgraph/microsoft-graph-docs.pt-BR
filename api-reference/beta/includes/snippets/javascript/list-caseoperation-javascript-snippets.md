---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad728521a2162d07aebe550ec6fd7a34bc9767c5
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094165"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let operations = await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/operations')
    .version('beta')
    .get();

```