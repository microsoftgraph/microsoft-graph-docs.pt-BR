---
title: Tipo de recurso apiAuthenticationConfigurationBase
description: Representa o tipo base de configuração de autenticação usado para chamar uma API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 915e1c0c26cee173991d75bc46a1a0230844d2ec
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507963"
---
# <a name="apiauthenticationconfigurationbase-resource-type"></a>Tipo de recurso apiAuthenticationConfigurationBase

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
