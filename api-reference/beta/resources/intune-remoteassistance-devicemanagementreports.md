---
title: Tipo de recurso deviceManagementReports
description: Classe DeviceManagementReports para Reporting V2
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e3d743244ffd4d54703ff74426008835e62e0e0d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039487"
---
# <a name="devicemanagementreports-resource-type"></a>Tipo de recurso deviceManagementReports

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Classe DeviceManagementReports para Reporting V2

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagementReports](../api/intune-remoteassistance-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-remoteassistance-devicemanagementreports.md)|Leia propriedades e relações do [objeto deviceManagementReports.](../resources/intune-remoteassistance-devicemanagementreports.md)|
|[Atualizar deviceManagementReports](../api/intune-remoteassistance-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-remoteassistance-devicemanagementreports.md)|Atualize as propriedades de [um objeto deviceManagementReports.](../resources/intune-remoteassistance-devicemanagementreports.md)|
|[ação getRemoteAssistanceSessionsReport](../api/intune-remoteassistance-devicemanagementreports-getremoteassistancesessionsreport.md)|Fluxo|Ainda não documentado|
|[ação getRemoteAssistanceMonitorActiveSessionsReport](../api/intune-remoteassistance-devicemanagementreports-getremoteassistancemonitoractivesessionsreport.md)|Fluxo|Ainda não documentado|
|[ação getRemoteAssistanceMonitorTotalSessionsReport](../api/intune-remoteassistance-devicemanagementreports-getremoteassistancemonitortotalsessionsreport.md)|Fluxo|Ainda não documentado|
|[ação getRemoteAssistanceMonitorAvgSessionTimeReport](../api/intune-remoteassistance-devicemanagementreports-getremoteassistancemonitoravgsessiontimereport.md)|Fluxo|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave da entidade|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReports"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "String (identifier)"
}
```



