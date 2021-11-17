---
title: Tipo de recurso keyCredentialConfiguration
description: Tipo complexo de configuração de credenciais de chave para configurar a restrição de credenciais de chave, maxLifetime e data de imposição
ms.localizationpriority: medium
author: madansr7
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 05fc7bab3a5073032ca3d27fd63424ff5b6fea56
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044782"
---
# <a name="keycredentialconfiguration-resource-type"></a>Tipo de recurso keyCredentialConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Objeto de configuração de credenciais chave que contém propriedades para configurar restrições, como restringir o tempo de vida dos segredos principais.

## <a name="properties"></a>Propriedades

| Propriedade                            | Tipo                                                                               | Descrição                                                                                                                                                                                                                                                                                   |
| :---------------------------------- | :--------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| restrictionType                     | appKeyCredentialRestrictionType | O tipo de restrição que está sendo aplicado. Os valores possíveis `asymmetricKeyLifetime` são , `unknownFutureValue` . Cada valor de restrictionType pode ser usado apenas uma vez por política.                                                                                                                        |
| maxLifeTime                         | Duração                                                                           |Valor que pode ser usado como a duração máxima em dias, horas, minutos ou segundos a partir da data de criação da chave, para a qual a chave é válida.  Definido no formato ISO 8601 para Durações. Por exemplo, `P4DT12H30M5S` representa uma duração de quatro dias, doze horas, trinta minutos e cinco segundos. Essa propriedade é necessária quando **restrictionType** é definido como `keyLifetime` . |
| restrictForAppsCreatedAfterDateTime | DateTimeOffset                                                                     | Data/hora em que a política é imposta para todos os aplicativos criados na ou após a data especificada. Para aplicativos existentes, a data de aplicação seria datada de volta. Para aplicar a todos os aplicativos, independentemente da data de criação, essa propriedade seria `null` . Anulável. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyCredentialConfiguration"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.keyCredentialConfiguration",
  "restrictionType": {
    "@odata.type": "microsoft.graph.appKeyCredentialRestrictionType"
  },
  "maxLifetime": "String (duration)",
  "restrictForAppsCreatedAfterDateTime": "DateTimeOffset"
}
```
