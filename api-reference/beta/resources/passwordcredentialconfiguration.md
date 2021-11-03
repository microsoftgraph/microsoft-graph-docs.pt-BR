---
title: Tipo de recurso passwordCredentialConfiguration
description: Tipo complexo de configuração de credencial de senha para configurar restrição de credencial de senha, maxLifetime e data de imposição
author: madansr7
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7789a2251517e881850e1a6fd732253894492e13
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697134"
---
# <a name="passwordcredentialconfiguration-resource-type"></a>Tipo de recurso passwordCredentialConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Objeto de configuração de credencial de senha que contém propriedades para configurar restrições, como bloqueio ou restrição de vida útil de segredos de senha.

## <a name="properties"></a>Propriedades

| Propriedade                            | Tipo                                                                               | Descrição                                                                                                                                                                                                                                                                                   |
| :---------------------------------- | :--------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| restrictionType                     | appCredentialRestrictionType |  O tipo de restrição que está sendo aplicado. Os valores possíveis são: `passwordAddition`, `passwordLifetime`, `symmetricKeyAddition`, `symmetricKeyLifetime`, `unknownFutureValue`. Cada valor de restrictionType pode ser usado apenas uma vez por política. |
| maxLifeTime                         | Duração                                                                           | Valor que pode ser usado como o número máximo para definir o tempo de expiração da senha em dias, horas, minutos ou segundos. Por exemplo, "P4DT12H30M5S" representa uma duração de quatro dias, doze horas, trinta minutos e cinco segundos. Essa propriedade é necessária quando o tipo de restrição é definido como `passwordLifetime` . |
| restrictForAppsCreatedAfterDateTime | DateTimeOffset                                                                     | Impõe a política para um aplicativo criado na ou após a data de aplicação. Para aplicativos existentes, a data de aplicação seria datada de volta. Para aplicar a todos os aplicativos, o tempo de data de imposição seria nulo.                                                                               |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.passwordCredentialConfiguration"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.passwordCredentialConfiguration",
  "restrictionType": {
    "@odata.type": "microsoft.graph.appCredentialRestrictionType"
  },
  "maxLifetime": "String (duration)",
  "restrictForAppsCreatedAfterDateTime": "DateTimeOffset"
}
```
