---
title: Tipo de recurso cloudPcReviewStatus
description: Representa detalhes sobre o status de revisão de um PC na nuvem.
author: yayang3
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: efaaeeab9474ab785cba4f40e64794af6d3344fc
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629492"
---
# <a name="cloudpcreviewstatus-resource-type"></a>Tipo de recurso cloudPcReviewStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes sobre o status de revisão de um PC na nuvem.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|azureStorageAccountId|Cadeia de caracteres|A ID do recurso da conta de Armazenamento do Azure na qual o instantâneo do PC na nuvem está sendo salvo.|
|azureStorageAccountName|Cadeia de caracteres|O nome da conta de Armazenamento do Azure na qual o instantâneo do PC na nuvem está sendo salvo.|
|inReview|Booleano| `True` se o PC na nuvem estiver definido como em revisão pelo administrador.|
|restorePointDateTime|DateTimeOffset|A data e a hora específicas do instantâneo do PC na nuvem que foi tirado e salvo automaticamente, quando o PC na nuvem é definido como em revisão. O carimbo de data/hora é mostrado no formato ISO 8601 e no UTC (Tempo Universal Coordenado). Por exemplo, meia-noite UTC em 1º de janeiro de 2014 aparece como `2014-01-01T00:00:00Z`.|
|reviewStartDateTime|DateTimeOffset|A data e a hora específicas em que o PC na nuvem foi definido em revisão. O carimbo de data/hora é mostrado no formato ISO 8601 e no UTC (Tempo Universal Coordenado). Por exemplo, meia-noite UTC em 1º de janeiro de 2014 aparece como `2014-01-01T00:00:00Z`.|
|subscriptionId|Cadeia de Caracteres|A ID da assinatura do Azure na qual o instantâneo do PC na nuvem está sendo salvo, no formato GUID.|
|subscriptionName|Cadeia de caracteres|O nome da assinatura do Azure na qual o instantâneo do PC na nuvem está sendo salvo.|
|userAccessLevel|[cloudPcUserAccessLevel](#cloudpcuseraccesslevel-values)|O nível de acesso do usuário final no PC na nuvem. Os valores possíveis são: `unrestricted` e `restricted`.|

### <a name="cloudpcuseraccesslevel-values"></a>Valores cloudPcUserAccessLevel

|Membro|Valor|Descrição|
|:---|:---|:---|
|irrestrito|0|Sem restrição. Os usuários podem acessar o PC na nuvem.|
|Restrito|1|Os usuários não têm permissão para acessar o PC na nuvem.|
|unknownFutureValue|999|Valor de sentinel de enumeração evolvável. Não usar.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcReviewStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcReviewStatus",
  "azureStorageAccountId": "String",
  "azureStorageAccountName": "String",
  "inReview": "Boolean",
  "restorePointDateTime": "String (timestamp)",
  "reviewStartDateTime": "String (timestamp)",
  "subscriptionId": "String",
  "subscriptionName": "String",
  "userAccessLevel": "String"
}
```

