---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 523057b3050b203240af9f607b7e10757ab7126e
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37636924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tentativelyAccept = {
  comment: "I may not be able to make this week. How about next week?",
  sendResponse: true,
  proposedNewTime: {
      start: { 
          dateTime: "2019-12-02T18:00:00", 
          timeZone: "Pacific Standard Time" 
      }, 
      end: { 
          dateTime: "2019-12-02T19:00:00", 
          timeZone: "Pacific Standard Time" 
      }     
  }
};

let res = await client.api('/me/events/{id}/tentativelyAccept')
    .version('beta')
    .post(tentativelyAccept);

```