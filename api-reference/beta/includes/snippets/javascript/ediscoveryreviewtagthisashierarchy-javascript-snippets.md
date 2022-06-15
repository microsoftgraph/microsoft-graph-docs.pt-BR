---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 781e8f9930a508a49ecdfb0dba633b48d20f69ef
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let asHierarchy = await client.api('/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags/asHierarchy')
    .version('beta')
    .get();

```