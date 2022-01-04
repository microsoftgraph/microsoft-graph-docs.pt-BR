---
title: Tipo de recurso androidDeviceOwnerSystemUpdateFreezePeriod
description: Representa um item na lista de períodos de congelamento para atualizações do sistema proprietário do dispositivo Android
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 54c3d150a579f981eccbe03dfccddfaf8b02b701
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/04/2022
ms.locfileid: "61712141"
---
# <a name="androiddeviceownersystemupdatefreezeperiod-resource-type"></a>Tipo de recurso androidDeviceOwnerSystemUpdateFreezePeriod

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um item na lista de períodos de congelamento para atualizações do sistema proprietário do dispositivo Android

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startMonth|Int32|O mês da data de início do período de congelamento. Valores válidos de 1 a 12|
|startDay|Int32|O dia da data de início do período de congelamento. Valores válidos de 1 a 31|
|endMonth|Int32|O mês da data de término do período de congelamento. Valores válidos de 1 a 12|
|endDay|Int32|O dia da data de término do período de congelamento. Valores válidos de 1 a 31|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod",
  "startMonth": 1024,
  "startDay": 1024,
  "endMonth": 1024,
  "endDay": 1024
}
```




