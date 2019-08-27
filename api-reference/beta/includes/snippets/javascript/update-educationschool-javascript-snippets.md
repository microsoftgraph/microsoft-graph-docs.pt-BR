---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d02e4d7fe379f9b07dab3a4e7175f1cfbe2d9200
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636091"
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

let res = await client.api('/education/schools/10002')
    .version('beta')
    .update(educationSchool);

```