---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e0cc0b41451615b543d088c545552eb54fa75033dce4d4e81df6d9d685fa64d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101546"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  displayName: 'Rogelio Cazares',
  givenName: 'Rogelio',
  middleName: 'Fernando',
  surname: 'Cazares',
};

await client.api('/education/users/{user-id}')
    .update(educationUser);

```