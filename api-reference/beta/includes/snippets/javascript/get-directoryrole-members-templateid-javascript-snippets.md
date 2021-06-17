---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71283c7ea9ccc826993cca4101e83a7f43286944
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990861"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members')
    .version('beta')
    .get();

```