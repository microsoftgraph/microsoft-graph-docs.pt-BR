---
title: tipo de recurso userAccountInformation
description: tipo de recurso userAccountInformation
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0bdb0bd3856e8eaf55d19d01a8566a34810051c7
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949486"
---
# <a name="useraccountinformation-resource-type"></a>tipo de recurso userAccountInformation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações especificamente ligadas à conta de um usuário, seja ela uma conta do Azure AD ou uma conta da Microsoft. O identificador de entidade é definido como o GUID do Azure AD correspondente ou o CID da conta da Microsoft, respectivamente. Esses campos são somente leitura por meio do Microsoft Graph e devem ser editados por meio de um perfil de usuário ou por um administrador de locatários em uma experiência correspondente.

Herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

| Método                                                             | Tipo de retorno                                         | Descrição                                                         |
|:-------------------------------------------------------------------|:----------------------------------------------------|:--------------------------------------------------------------------|
| [Obter userAccountInformation](../api/useraccountinformation-get.md) | [userAccountInformation](useraccountinformation.md) | Leia as propriedades e os relacionamentos de um objeto **userAccountInformation** . |

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                       | Descrição                                                                                                                              |
|:--------------------|:---------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------|
|ageGroup             |String                      | Mostra o grupo de idade do usuário. Os valores `null`permitidos `minor`, `notAdult` e `adult` são gerados pelo diretório e não podem ser alterados.|
|countryCode          |Cadeia de caracteres|                     | Contém o código de país de dois caracteres associado à conta de usuários.                                                                |
|preferredLanguageTag |[localeInfo](localeinfo.md) | Contém o idioma que o usuário associou como preferencial para a conta.                                                              |
|userPrincipalName    |Cadeia de caracteres                      | O nome principal do usuário (UPN) do usuário associado à conta.                                                                   |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": ""
}-->

```json
{
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {"@odata.type": "microsoft.graph.localeInfo"},
  "userPrincipalName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAccountInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
