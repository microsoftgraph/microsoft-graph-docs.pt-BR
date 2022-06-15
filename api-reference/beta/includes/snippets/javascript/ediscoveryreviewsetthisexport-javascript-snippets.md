---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6fca1b3a381ff42831e69e33e2bce299617108f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _export = {
    outputName: 'Export via API',
    description: 'Export for the Contoso investigation',
    exportOptions: 'originalFiles,fileInfo,tags',
    exportStructure: 'directory'
};

await client.api('/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/export')
    .version('beta')
    .post(_export);

```