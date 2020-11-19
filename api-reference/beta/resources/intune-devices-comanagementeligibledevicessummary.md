---
title: tipo de recurso comanagementEligibleDevicesSummary
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4c7244bd594e38a8f129aa81389b159caff6b928
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214635"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a>tipo de recurso comanagementEligibleDevicesSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|comanagedCount|Int32|Contagem de dispositivos já Co-Managed|
|eligibleCount|Int32|Contagem de dispositivos totalmente qualificados para Co-Management|
|eligibleButNotAzureAdJoinedCount|Int32|Contagem de dispositivos qualificados para Co-Management, mas ainda não ingressaram no Azure Active Directory|
|needsOsUpdateCount|Int32|Contagem de dispositivos que serão qualificados para Co-Management após uma atualização de so|
|ineligibleCount|Int32|Contagem de dispositivos não qualificados para Co-Management|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagementEligibleDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevicesSummary",
  "comanagedCount": 1024,
  "eligibleCount": 1024,
  "eligibleButNotAzureAdJoinedCount": 1024,
  "needsOsUpdateCount": 1024,
  "ineligibleCount": 1024
}
```




