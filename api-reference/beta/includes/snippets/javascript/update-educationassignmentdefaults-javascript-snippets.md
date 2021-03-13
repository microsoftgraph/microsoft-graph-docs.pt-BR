---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9b631940036d11628b7110c8084fc667b43166f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804713"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignmentDefaults = {
  addedStudentAction: 'assignIfOpen',
  notificationChannelUrl: 'https://graph.microsoft.com/beta/teams(\'id\')/channels(\'id\')'
};

await client.api('/education/classes/{id}/assignmentDefaults')
    .version('beta')
    .update(educationAssignmentDefaults);

```