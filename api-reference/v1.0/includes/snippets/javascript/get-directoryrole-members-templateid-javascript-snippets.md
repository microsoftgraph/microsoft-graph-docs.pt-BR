---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7725fb8be7beae67e5cbc70476e574670450fadba48194e8cb68ebd8c670639a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215282"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members')
    .get();

```