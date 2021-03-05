---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9296741702c9e14ac554a5d5b28e77b8f88b118e
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470312"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignmentDefaults = {
  addedStudentAction: "assignIfOpen",
  notificationChannelUrl: "https://graph.microsoft.com/beta/teams('id')/channels('id')"
};

let res = await client.api('/education/classes/{id}/assignmentDefaults')
    .version('beta')
    .update(educationAssignmentDefaults);

```