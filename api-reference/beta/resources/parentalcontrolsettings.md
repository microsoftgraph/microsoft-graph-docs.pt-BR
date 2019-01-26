---
title: tipo de recurso de parentalControlSettings
description: Especifica as configurações de controle do responsável para um aplicativo. Essas configurações controlam a experiência de consentimento.
localization_priority: Normal
ms.openlocfilehash: 8a3a768cc9264b6d1a25532455da20d87a5bc4e8
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573869"
---
# <a name="parentalcontrolsettings-resource-type"></a>tipo de recurso de parentalControlSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica as configurações de controle do responsável para um aplicativo. Essas configurações controlam a experiência de consentimento.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
:---------------|:--------|:----------|
|countriesBlockedForMinors|String collection| Especifica os [códigos de país ISO de duas letras](https://www.iso.org/iso-3166-country-codes.html). Acesso ao aplicativo será bloqueado para menores dos países especificados na lista.|
|legalAgeGroupRule| String | Especifica a regra de grupo de idade legais que se aplica a usuários do aplicativo. Pode ser definido como um dos seguintes valores: <table><tr><th>Valor</th><th>Descrição</th></tr><tr><td>Permitir</td><td>Padrão. Impõe o mínimo legal. Isso significa que o consentimento dos pais é necessário para menores na União Europeia e Coreia.</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>Impõe o usuário para especificar a data de nascimento esteja em conformidade com as regras de COPPA. </td></tr><tr><td>RequireConsentForMinors</td><td>Requer o consentimento dos pais para anos abaixo 18, independentemente das regras de país secundárias.</td></tr><tr><td>RequireConsentForKids</td><td>Requer o consentimento dos pais para anos abaixo 14, independentemente das regras de país secundárias.</td></tr><tr><td>BlockMinors</td><td>Menores de blocos de usar o aplicativo.</td></tr></table> |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- 
{
    "blockType": "resource",
    "@odata.type":"microsoft.graph.parentalControlSettings"
}
-->
```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/parentalcontrolsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
