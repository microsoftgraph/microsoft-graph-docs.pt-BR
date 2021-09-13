---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2c273e1970b354ab922b9adf109944b3fd536401c7a09117272571c4fcd143e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnnotation = {
  detail: {
    contentType: 'text',
    content: 'I am originally from Australia, but grew up in Moscow, Russia.'
  },
  displayName: 'About Me'
};

await client.api('/me/profile/notes')
    .version('beta')
    .post(personAnnotation);

```