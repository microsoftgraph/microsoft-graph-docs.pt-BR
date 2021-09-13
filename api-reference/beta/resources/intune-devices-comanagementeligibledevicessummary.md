---
title: Tipo de recurso comanagementEligibleDevicesSummary
description: Ainda não documentado
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90f4cb5f33b0ea1c260d6b6acaffac46d3e08434
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111037"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a>Tipo de recurso comanagementEligibleDevicesSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|comanagedCount|Int32|Contagem de dispositivos já Co-Managed|
|eligibleCount|Int32|Contagem de dispositivos totalmente qualificados para Co-Management|
|eligibleButNotAzureAdJoinedCount|Int32|Contagem de dispositivos qualificados para Co-Management mas ainda não ingressados no Azure Active Directory|
|needsOsUpdateCount|Int32|Contagem de dispositivos que serão qualificados para Co-Management após uma atualização do sistema operacional|
|ineligibleCount|Int32|Contagem de dispositivos inelegíveis para Co-Management|

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



