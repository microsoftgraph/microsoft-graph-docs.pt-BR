---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2342dfc53e9a0c7e6d89885f8af9141d72aeafa1
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904532"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const place = {
  @odata.type: "microsoft.graph.roomList",
  displayName: "Building 1",
  phone:"555-555-0100",
  address: {
    street: "4567 Main Street",
    city: "Buffalo",
    state: "NY",
    postalCode: "98052",
    countryOrRegion: "USA"
  },
  geoCoordinates: {
    altitude: null,
    latitude: 47.0,
    longitude: -122.0,
    accuracy: null,
    altitudeAccuracy: null
 }
};

let res = await client.api('/places/Building1RroomList@contoso.onmicrosoft.com')
    .update(place);

```