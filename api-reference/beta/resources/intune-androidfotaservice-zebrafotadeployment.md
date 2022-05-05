---
title: Tipo de recurso zebraFotaDeployment
description: A entidade de implantação zebra FOTA que descreve as configurações, os grupos de dispositivos de implantação necessários para criar uma implantação fota e o status da implantação.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d3ba6ffd223320be5bfbe1b259768534a47941c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213055"
---
# <a name="zebrafotadeployment-resource-type"></a>Tipo de recurso zebraFotaDeployment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de implantação zebra FOTA que descreve as configurações, os grupos de dispositivos de implantação necessários para criar uma implantação fota e o status da implantação.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar zebraFotaDeployments](../api/intune-androidfotaservice-zebrafotadeployment-list.md)|[Coleção zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md)|Listar propriedades e relações dos objetos [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) .|
|[Obter zebraFotaDeployment](../api/intune-androidfotaservice-zebrafotadeployment-get.md)|[zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md)|Ler propriedades e relações do objeto [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) .|
|[Criar zebraFotaDeployment](../api/intune-androidfotaservice-zebrafotadeployment-create.md)|[zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md)|Crie um novo [objeto zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) .|
|[Excluir zebraFotaDeployment](../api/intune-androidfotaservice-zebrafotadeployment-delete.md)|Nenhuma|Exclui um [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md).|
|[Atualizar zebraFotaDeployment](../api/intune-androidfotaservice-zebrafotadeployment-update.md)|[zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md)|Atualize as propriedades de um [objeto zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) .|
|[ação de cancelamento](../api/intune-androidfotaservice-zebrafotadeployment-cancel.md)|Booliano|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID de implantação gerada pelo sistema fornecida durante a criação da implantação. Retornado somente se a operação tiver sido bem-sucedida.|
|displayName|Cadeia de caracteres|Um nome legível por humanos da implantação.|
|descrição|Cadeia de caracteres|Uma descrição legível humana da implantação.|
|deploymentSettings|[zebraFotaDeploymentSettings](../resources/intune-androidfotaservice-zebrafotadeploymentsettings.md)|Representa as configurações necessárias para criar uma implantação, como tipo de implantação, informações de artefato, download e instalação|
|deploymentAssignments|[coleção androidFotaDeploymentAssignment](../resources/intune-androidfotaservice-androidfotadeploymentassignment.md)|Coleção de atribuição de FOTA do Android|
|Deploymentstatus|[zebraFotaDeploymentStatus](../resources/intune-androidfotaservice-zebrafotadeploymentstatus.md)|Representa o status de implantação da Zebra. O status é um status de alto nível da implantação, em vez de ser um status detalhado por dispositivo.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.zebraFotaDeployment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaDeployment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "deploymentSettings": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentSettings",
    "deviceModel": "String",
    "updateType": "String",
    "timeZoneOffsetInMinutes": 1024,
    "firmwareTargetBoardSupportPackageVersion": "String",
    "firmwareTargetPatch": "String",
    "firmwareTargetOsVersion": "String",
    "scheduleMode": "String",
    "scheduleDurationInDays": 1024,
    "downloadRuleNetworkType": "String",
    "downloadRuleStartDateTime": "String (timestamp)",
    "installRuleStartDateTime": "String (timestamp)",
    "installRuleWindowStartTime": "String (time of day)",
    "installRuleWindowEndTime": "String (time of day)",
    "batteryRuleMinimumBatteryLevelPercentage": 1024,
    "batteryRuleRequireCharger": true
  },
  "deploymentAssignments": [
    {
      "@odata.type": "microsoft.graph.androidFotaDeploymentAssignment",
      "id": "String",
      "target": {
        "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget",
        "groupId": "String"
      }
    }
  ],
  "deploymentStatus": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentStatus",
    "state": "String",
    "totalDevices": 1024,
    "totalCreated": 1024,
    "totalScheduled": 1024,
    "totalDownloading": 1024,
    "totalAwaitingInstall": 1024,
    "totalSucceededInstall": 1024,
    "totalCanceled": 1024,
    "totalUnknown": 1024,
    "totalFailedDownload": 1024,
    "totalFailedInstall": 1024,
    "completeOrCanceledDateTime": "String (timestamp)",
    "cancelRequested": true,
    "lastUpdatedDateTime": "String (timestamp)"
  }
}
```




