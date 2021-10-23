---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef187056d9d2ac453a0477f129fb907e53ab493f
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559135"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const meetingRegistrationQuestion = {
  displayName: 'What\'s your job position?',
  isRequired: false,
  answerInputType: 'text'
};

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/customQuestions')
    .version('beta')
    .post(meetingRegistrationQuestion);

```