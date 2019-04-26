---
title: tipo de recurso parentalControlSettings
description: Especifica as configurações de controle parental de um aplicativo. Essas configurações controlam a experiência de consentimento.
localization_priority: Normal
ms.openlocfilehash: 8e62e137b872437626a5c77c114f14c6ad0c5eb2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344959"
---
# <a name="parentalcontrolsettings-resource-type"></a>tipo de recurso parentalControlSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica as configurações de controle parental de um aplicativo. Essas configurações controlam a experiência de consentimento.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
:---------------|:--------|:----------|
|countriesBlockedForMinors|Coleção String| Especifica os [códigos de país ISO de duas letras](https://www.iso.org/iso-3166-country-codes.html). O acesso ao aplicativo será bloqueado para menores dos países especificados nesta lista.|
|legalAgeGroupRule| String | Especifica a regra de grupo de idades legais que se aplica aos usuários do aplicativo. Pode ser definido como um dos seguintes valores: <table><tr><th>Valor</th><th>Descrição</th></tr><tr><td>Permitir</td><td>Padrão. Impõe o mínimo legal. Isso significa que o consentimento do responsável é obrigatório para menores na União Européia e na Coréia.</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>Impõe que o usuário especifique a data de nascimento para estar em conformidade com as regras do COOPA. </td></tr><tr><td>RequireConsentForMinors</td><td>Requer o consentimento dos pais para crianças abaixo de 18, independentemente das regras secundárias do país.</td></tr><tr><td>RequireConsentForKids</td><td>Requer o consentimento dos pais para crianças abaixo de 14, independentemente das regras secundárias do país.</td></tr><tr><td>BlockMinors</td><td>Bloqueia os menores de usar o aplicativo.</td></tr></table> |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.parentalControlSettings"
}-->
```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
