---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2b70df4587d8cba0c9a43d45f728b001fcecd4356e45cfe43686edd0992b3c6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158120"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tentativelyAccept = {
  comment: 'I may not be able to make this week. How about next week?',
  sendResponse: true,
  proposedNewTime: {
      start: { 
          dateTime: '2019-12-02T18:00:00', 
          timeZone: 'Pacific Standard Time' 
      }, 
      end: { 
          dateTime: '2019-12-02T19:00:00', 
          timeZone: 'Pacific Standard Time' 
      }     
  }
};

await client.api('/me/events/{id}/tentativelyAccept')
    .post(tentativelyAccept);

```