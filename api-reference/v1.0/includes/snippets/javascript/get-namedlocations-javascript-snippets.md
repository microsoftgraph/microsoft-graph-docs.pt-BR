---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 939d7e4f8e514a1994da830ad180f1cec0276c80
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566018"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/conditionalAccess/namedLocations')
    .filter('microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')')
    .get();

```