---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2c5d415eeb36a72056f08b408f5380d2c878492
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  displayName: "Rogelio Cazares",
  givenName: "Rogelio",
  middleName: "Fernando",
  surname: "Cazares",
};

let res = await client.api('/education/users/13020')
    .version('beta')
    .update({educationUser : educationUser});

```