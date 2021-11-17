---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fac49ce8eb8a71678b35193e1de899c3ea9e4815200fac35cadbe1a4aaab489d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pkcs12Value = "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA";

var password = "<password>";

await graphClient.Identity.ApiConnectors["{identityApiConnector-id}"]
    .UploadClientCertificate(pkcs12Value,password)
    .Request()
    .PostAsync();

```