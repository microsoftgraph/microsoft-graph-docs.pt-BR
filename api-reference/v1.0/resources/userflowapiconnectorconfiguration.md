---
title: Tipo de recurso userFlowApiConnectorConfiguration
description: Representa os conectores de API habilitados para um fluxo de usuários.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 474011cceb4c05e2c1b8f61aa4ea0e05e03df26857a0c10ea3a7197d453d24c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230414"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a>Tipo de recurso userFlowApiConnectorConfiguration

Namespace: microsoft.graph

Define as APIs que são chamadas em pontos específicos no fluxo do usuário.  Cada relação desse objeto corresponde a uma etapa específica no fluxo do usuário que pode ser configurada para chamar um conector de API.

## <a name="relationships"></a>Relações

| Relação            | Tipo                                            | Descrição                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| postFederationSignup    | [identityApiConnector](identityapiconnector.md) | Especifica uma API a ser chamada após a federação com um provedor de identidade externo. Por exemplo, uma API do Google, Facebook ou Azure AD é concluída quando o usuário está se insinuando (não se aplica à inscrição). |
| postAttributeCollection | [identityApiConnector](identityapiconnector.md) | Especifica uma API a ser chamada depois que um usuário envia os atributos coletados e antes que a conta de usuário seja criada durante a assinatura.                                                      |

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
