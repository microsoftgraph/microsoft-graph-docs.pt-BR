---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96ae1fb399de6b56aa1612a6332cf5c921225557350d72667254f7573a7a2e7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let languages = await client.api('/identity/b2xUserFlows/B2X_1_PartnerSignUp/languages')
    .get();

```