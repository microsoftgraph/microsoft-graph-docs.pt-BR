---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2e9bd0a8bb85357f29cf969be0b7bc6d2ef15d6fa9b1f54ed573e706b01509c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  displayName: 'Architecture Discussion',
  description: 'This channel is where we debate all future architecture plans',
  membershipType: 'standard'
};

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels')
    .post(channel);

```