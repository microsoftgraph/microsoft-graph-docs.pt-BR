---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76419dca367f527c6d061a90607d59151563c2d19465fcd2b10f8ca8b8fd8ad0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102151"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  parentFolderId: 'parentFolderId-value',
  birthday: '2016-10-19T10:37:00Z',
  fileAs: 'fileAs-value',
  displayName: 'displayName-value',
  givenName: 'givenName-value',
  initials: 'initials-value'
};

await client.api('/me/contactFolders/{id}/contacts')
    .version('beta')
    .post(contact);

```