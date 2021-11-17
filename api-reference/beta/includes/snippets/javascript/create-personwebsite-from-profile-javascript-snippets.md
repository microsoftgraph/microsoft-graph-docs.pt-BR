---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0f6c80e2195ec5399dcde2cbcaabbe0db3342282f5d87daa6d2a74fb0c396b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159766"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personWebsite = {
  categories: [
    'football'
  ],
  displayName: 'Lyn Damer',
  webUrl: 'www.lyndamer.no'
};

await client.api('/me/profile/websites')
    .version('beta')
    .post(personWebsite);

```