---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6cda4e5675ced530b5e018a6ed62b6036bb16804
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732763"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSchool = {
  displayName: "Fabrikam Arts High School",
  description: "Magnate school for the arts. Los Angeles School District"
};

let res = await client.api('/education/schools/{school-id}')
    .update({educationSchool : educationSchool});

```