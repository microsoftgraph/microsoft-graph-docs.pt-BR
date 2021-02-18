---
title: Tipo de recurso userFlowApiConnectorConfiguration
description: Representa quais conectores de API estão habilitados para um fluxo de usuário.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 78e93f4b743f57a68faad530f2a26ad6dead8a08
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292881"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a>Tipo de recurso userFlowApiConnectorConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define quais APIs são chamadas em pontos específicos no fluxo do usuário.  Cada relação desse objeto corresponde a uma etapa específica no fluxo do usuário que pode ser configurada para chamar um conector de API.

## <a name="relationships"></a>Relações

| Relação            | Tipo                                            | Descrição                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| postFederationSignup    | [identityApiConnector](identityapiconnector.md) | Especifica uma API para chamar após a federação com um provedor de identidade externo (como Google, Facebook ou Azure AD) é concluída quando o usuário está se insinndo (não se aplica a entrar). |
| postAttributeCollection | [identityApiConnector](identityapiconnector.md) | Especifica uma API a ser chamada depois que um usuário envia atributos coletados e antes de o usuário ser criado durante a assinatura.                                                      |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowApiConnectorConfiguration"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "User flow API Connector Configuration",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
