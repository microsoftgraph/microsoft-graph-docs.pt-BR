---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efe529a966aae83f9426d42482234752b2092436
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963952"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const namedLocation = {
    '@odata.type': '#microsoft.graph.countryNamedLocation',
    displayName: 'Named location with unknown countries and regions',
    countriesAndRegions: [
        'US',
        'GB'
    ],
    includeUnknownCountriesAndRegions: true
};

await client.api('/identity/conditionalAccess/namedLocations')
    .post(namedLocation);

```