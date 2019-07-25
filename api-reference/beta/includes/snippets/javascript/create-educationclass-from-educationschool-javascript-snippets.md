---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cef07a40c27b4fd3ccccd16fe1daffc1fe9dfe5e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
 @odata.id:"https://graph.microsoft.com/beta/education/classes/11006"
};

let res = await client.api('/education/schools/10002/classes/$ref')
    .version('beta')
    .post({educationClass : educationClass});

```