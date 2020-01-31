---
title: tipo de recurso comanagementEligibleSummaryEntity
description: tipo de recurso comanagementEligibleSummaryEntity
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80c2afff56d845097990ef927a743678a248c9fd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636578"
---
# <a name="comanagementeligiblesummaryentity-resource-type"></a>tipo de recurso comanagementEligibleSummaryEntity

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar comanagementEligibleSummaryEntity](../api/intune-device-comanagementEligibleSummaryEntity-list.md)|coleção comanagementEligibleSummaryEntity|Listar Propriedades e relações dos objetos comanagementEligibleSummaryEntity.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID exclusiva do EligibleDeviceSummaryEntity|
|coManagedCount|Int32|Contagem de dispositivos já cogerenciados|
|eligibleCount|Int32|Contagem de dispositivos totalmente qualificados para o cogerenciamento|
|eligibleButNotAadJoinedCount|Int32|Contagem de dispositivos qualificados para o cogerenciamento, mas ainda não ingressou no Azure Active Directory|
|needsOSUpdateCount|Int32|Contagem de dispositivos que serão qualificados para cogerenciamento após uma atualização de so|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleSummaryEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleSummaryEntity",
  "id": "String (identifier)",
  "coManagedCount": 1024,
  "eligibleCount": 1024,
  "eligibleButNotAadJoinedCount": 1024,
  "needsOSUpdateCount": 1024
}
```

