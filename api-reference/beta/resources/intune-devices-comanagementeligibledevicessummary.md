---
title: tipo de recurso comanagementEligibleDevicesSummary
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 55df0591dfcbabd997dfda1bb07dbd116c14dcbe
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793448"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a>tipo de recurso comanagementEligibleDevicesSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|comanagedCount|Int32|Contagem de dispositivos já cogerenciados|
|eligibleCount|Int32|Contagem de dispositivos totalmente qualificados para o cogerenciamento|
|eligibleButNotAzureAdJoinedCount|Int32|Contagem de dispositivos qualificados para cogerenciamento, mas ainda não ingressou no Azure Active Directory|
|needsOsUpdateCount|Int32|Contagem de dispositivos que serão qualificados para cogerenciamento após uma atualização de so|
|ineligibleCount|Int32|Contagem de dispositivos não qualificados para cogerenciamento|

## <a name="relationships"></a>Relações
Nenhuma

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



