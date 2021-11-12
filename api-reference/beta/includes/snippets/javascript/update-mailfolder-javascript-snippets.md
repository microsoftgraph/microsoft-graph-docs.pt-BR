---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4bf9dbe7fd8b18c885bbd66f51bbce544f2bb1126937121e451e21c2a078da3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160180"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: 'displayName-value',
};

await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .version('beta')
    .update(mailFolder);

```