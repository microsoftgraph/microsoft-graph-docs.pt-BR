---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8c96eb020184d5ebe858b0f5a34800a6ad26ecf461e3f18d920fb53d4d3ee03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159594"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon/hostedContent/$value')
    .version('beta')
    .get();

```