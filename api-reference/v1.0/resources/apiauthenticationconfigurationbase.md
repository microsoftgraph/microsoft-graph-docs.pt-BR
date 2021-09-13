---
title: Tipo de recurso apiAuthenticationConfigurationBase
description: Representa o tipo base de configuração de autenticação usado para chamar uma API.
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3e3086ac90eabc15527a84f9c215659def06b7ea
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094475"
---
# <a name="apiauthenticationconfigurationbase-resource-type"></a>Tipo de recurso apiAuthenticationConfigurationBase

Namespace: microsoft.graph

O tipo base para manter informações de autenticação para chamar uma API.

Os tipos derivados incluem:
- [basicAuthentication para](basicauthentication.md) autenticação básica HTTP
- [pkcs12certificate para autenticação](pkcs12certificate.md) de certificado do cliente (usado para criar ou carregar conectores de API)
- [clientCertificateAuthentication para](pkcs12certificate.md) autenticação de certificado de cliente (usado para buscar os certificados do cliente de um conector de API)

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.apiAuthenticationConfigurationBase"
}
```
