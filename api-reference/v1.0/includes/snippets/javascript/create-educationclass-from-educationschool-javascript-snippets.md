---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad6acf858672c7db56715ad8d3224b6ae4da1f57
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465469"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
 @odata.id:"https://graph.microsoft.com/v1.0/education/classes/11006"
};

let res = await client.api('/education/schools/{school-id}/classes/$ref')
    .post({educationClass : educationClass});

```