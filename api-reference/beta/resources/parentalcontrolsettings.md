---
title: Tipo de recurso parentalControlSettings
description: Especifica as configurações de controle parental de um aplicativo. Essas configurações controlam a experiência de consentimento.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f63f81af9e35183a15ab07b1f8e8fce9e8488bae
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135998"
---
# <a name="parentalcontrolsettings-resource-type"></a>Tipo de recurso parentalControlSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica as configurações de controle parental de um aplicativo. Essas configurações controlam a experiência de consentimento.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
:---------------|:--------|:----------|
|countriesBlockedForMinors|Coleção de cadeias de caracteres| Especifica os códigos [de país ISO de](https://www.iso.org/iso-3166-country-codes.html)duas letras. O acesso ao aplicativo será bloqueado para menores dos países especificados nesta lista.|
|legalAgeGroupRule| String | Especifica a regra de faixa etária legal que se aplica aos usuários do aplicativo. Pode ser definido como um dos seguintes valores: <table><tr><th>Valor</th><th>Descrição</th></tr><tr><td>Permitir</td><td>Padrão. Impõe o mínimo legal. Isso significa que o consentimento dos pais é necessário para menores na União Europeia e na Coreia.</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>Impõe que o usuário especifique a data de nascimento para estar em conformidade com as regras do COPPA. </td></tr><tr><td>RequireConsentForMinors</td><td>Requer o consentimento dos pais para menores de 18 anos, independentemente das regras secundárias do país.</td></tr><tr><td>RequireConsentForKids</td><td>Requer o consentimento dos pais para menores de 14 anos, independentemente das regras secundárias do país.</td></tr><tr><td>BlockMinors</td><td>Impede que menores usem o aplicativo.</td></tr></table> |

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


