---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5d87d599b3310301ebeebc9721d696d5c152f24f4b5202baec01afcddb339c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159714"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const answer = {
  callbackUri: 'https://bot.contoso.com/api/calls',
  acceptedModalities: [ 'audio' ],
  mediaConfig: {
    '@odata.type': '#microsoft.graph.appHostedMediaConfig',
    blob: '<Media Session Configuration Blob>'
  }
};

await client.api('/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/answer')
    .version('beta')
    .post(answer);

```