---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9d2134636baf82f2de7fc8a137c2b8b9b4c2a62e
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920444"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = {
LocalizedStrings: [
      {
          ElementType: 'UxElement',
          ElementId: null,
          StringId: 'alert_message',
          Override: true,
          Value: 'Are you sure that you want to cancel entering your information?'
      }
  ]
};

await client.api('/identity/b2xUserFlows/B2X_1_Partner/languages/en/overridesPages/selfasserted1_1/$value')
    .put(stream);

```