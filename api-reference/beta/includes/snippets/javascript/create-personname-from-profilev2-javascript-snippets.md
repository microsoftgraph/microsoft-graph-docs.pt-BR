---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7c5ff9e096b5d809cd1adc75c6fe1105517d7490
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997782"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personName = {
  displayName: "displayName-value",
  first: "first-value",
  initials: "initials-value",
  last: "last-value",
  languageTag: "languageTag-value",
  maiden: "maiden-value"
};

let res = await client.api('/me/profile/names')
    .version('beta')
    .post(personName);

```