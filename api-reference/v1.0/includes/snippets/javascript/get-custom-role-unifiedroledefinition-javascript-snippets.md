---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebf1b01cc589bef7ff2a05b0640894da6cedbb14
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59097829"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleDefinition = await client.api('/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a')
    .get();

```