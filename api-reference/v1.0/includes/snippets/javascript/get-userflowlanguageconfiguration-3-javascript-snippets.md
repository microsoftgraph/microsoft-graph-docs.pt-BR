---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2f28b209b4cb74c6fe3384a4f4e980923e109558976d5ee01a66cf94ee739eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275278"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlowLanguageConfiguration = await client.api('/identity/b2xUserFlows/B2X_1_Partner/languages/en')
    .get();

```