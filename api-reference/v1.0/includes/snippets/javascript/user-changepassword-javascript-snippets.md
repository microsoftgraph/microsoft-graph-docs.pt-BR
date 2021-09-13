---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c06f93e7e9a91aa26dddaab0c57fb28c933bfd3b9e8c1c16fdfb4a502f31052e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216810"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const changePassword = {
    currentPassword: 'xWwvJ]6NMw+bWH-d',
    newPassword: '0eM85N54wFxWwvJ]'
};

await client.api('/me/changePassword')
    .post(changePassword);

```