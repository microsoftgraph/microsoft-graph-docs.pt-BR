---
title: tipo de recurso de parentalControlSettings
description: Especifica as configurações de controle do responsável para um aplicativo. Essas configurações controlam a experiência de consentimento.
localization_priority: Normal
ms.openlocfilehash: bb6f776d5f206fb0ed35a999effc7bbdc0768512
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806514"
---
# <a name="parentalcontrolsettings-resource-type"></a>tipo de recurso de parentalControlSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Especifica as configurações de controle do responsável para um aplicativo. Essas configurações controlam a experiência de consentimento.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
:---------------|:--------|:----------|
|countriesBlockedForMinors|String collection| Especifica os [códigos de país ISO de duas letras](https://www.iso.org/iso-3166-country-codes.html). Acesso ao aplicativo será bloqueado para menores dos países especificados na lista.|
|legalAgeGroupRule| Cadeia de caracteres | Especifica a regra de grupo de idade legais que se aplica a usuários do aplicativo. Pode ser definido como um dos seguintes valores: <table><tr><th>Valor</th><th>Descrição</th></tr><tr><td>Permitir</td><td>Padrão. Impõe o mínimo legal. Isso significa que o consentimento dos pais é necessário para menores na União Europeia e Coreia.</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>Impõe o usuário para especificar a data de nascimento esteja em conformidade com as regras de COPPA. </td></tr><tr><td>RequireConsentForMinors</td><td>Requer o consentimento dos pais para anos abaixo 18, independentemente das regras de país secundárias.</td></tr><tr><td>RequireConsentForKids</td><td>Requer o consentimento dos pais para anos abaixo 14, independentemente das regras de país secundárias.</td></tr><tr><td>BlockMinors</td><td>Menores de blocos de usar o aplicativo.</td></tr></table> |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
