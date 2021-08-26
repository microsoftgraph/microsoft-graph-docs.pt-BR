---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04681c73bbbfb9cbde0e9c4a5dd9992b55c494f3da37c68fc0ac25bb23d51a97
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216480"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  destinationId: 'destinationId-value'
};

await client.api('/me/messages/{id}/copy')
    .post(message);

```