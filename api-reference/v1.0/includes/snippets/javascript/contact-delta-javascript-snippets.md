---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2cd945556cf542085a742ecd641a5ed8a79277db
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610413"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}/contacts/delta')
    .header('Prefer','odata.maxpagesize=2')
    .select('displayName')
    .get();

```