---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97a05953b0295d865d14d08961ccd7463b7d61f6
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780776"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getApplicableContentTypesForList = await client.api('/sites/{siteId}/getApplicableContentTypesForList(listId='{list-id}')')
    .get();

```