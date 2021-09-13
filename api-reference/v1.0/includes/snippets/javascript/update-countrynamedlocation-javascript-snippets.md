---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33e8e397532710054df1fadcc768224f1077cfa92287ce9743a55276288c195c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329469"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const namedLocation = {
    '@odata.type': '#microsoft.graph.countryNamedLocation',
    displayName: 'Updated named location without unknown countries and regions',
    countriesAndRegions: [
        'CA',
        'IN'
    ],
    includeUnknownCountriesAndRegions: false
};

await client.api('/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959')
    .update(namedLocation);

```