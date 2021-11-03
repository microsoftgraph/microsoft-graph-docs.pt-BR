---
title: Tipo de recurso keyCredentialConfiguration
description: Tipo complexo de configuração de credenciais de chave para configurar a restrição de credenciais de chave, maxLifetime e data de imposição
ms.localizationpriority: medium
author: madansr7
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: dbc208ec616f0b865cd848acdf932b045d215bf1
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688230"
---
# <a name="keycredentialconfiguration-resource-type"></a>Tipo de recurso keyCredentialConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Objeto de configuração de credenciais chave que contém propriedades para configurar restrições, como restringir o tempo de vida dos segredos principais.

## <a name="properties"></a>Propriedades

| Propriedade                            | Tipo                                                                               | Descrição                                                                                                                                                                                                                                                                                   |
| :---------------------------------- | :--------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| restrictionType                     | appKeyCredentialRestrictionType | O tipo de restrição que está sendo aplicado. Os valores possíveis `asymmetricKeyLifetime` são , `unknownFutureValue` . Cada valor de restrictionType pode ser usado apenas uma vez por política.                                                                                                                        |
| maxLifeTime                         | Duração                                                                           |Valor que pode ser usado como a duração máxima em dias, horas, minutos ou segundos a partir da data de criação da chave, para a qual a chave é válida. Por exemplo, `P4DT12H30M5S` representa uma duração de quatro dias, doze horas, trinta minutos e cinco segundos. Essa propriedade é necessária quando **restrictionType** é definido como `keyLifetime` . |
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
