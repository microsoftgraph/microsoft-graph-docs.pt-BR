---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51c8c74e83c6e2950049984905d5d83aeb6201e41d3da9f3ec196d11532c09ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214477"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamworkHostedContent = await client.api('/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon/hostedContent/')
    .version('beta')
    .get();

```