---
title: Criar zebraFotaDeployment
description: Crie um novo objeto zebraFotaDeployment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e9aa120d65788c0943e2e63e91758e3ec6a1dff4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212985"
---
# <a name="create-zebrafotadeployment"></a>Criar zebraFotaDeployment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/zebraFotaDeployments
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto zebraFotaDeployment.

A tabela a seguir mostra as propriedades que são necessárias ao criar o zebraFotaDeployment.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID de implantação gerada pelo sistema fornecida durante a criação da implantação. Retornado somente se a operação tiver sido bem-sucedida.|
|displayName|Cadeia de caracteres|Um nome legível por humanos da implantação.|
|descrição|Cadeia de caracteres|Uma descrição legível humana da implantação.|
|deploymentSettings|[zebraFotaDeploymentSettings](../resources/intune-androidfotaservice-zebrafotadeploymentsettings.md)|Representa as configurações necessárias para criar uma implantação, como tipo de implantação, informações de artefato, download e instalação|
|deploymentAssignments|[coleção androidFotaDeploymentAssignment](../resources/intune-androidfotaservice-androidfotadeploymentassignment.md)|Coleção de atribuição de FOTA do Android|
|Deploymentstatus|[zebraFotaDeploymentStatus](../resources/intune-androidfotaservice-zebrafotadeploymentstatus.md)|Representa o status de implantação da Zebra. O status é um status de alto nível da implantação, em vez de ser um status detalhado por dispositivo.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `201 Created` de resposta e um [objeto zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/zebraFotaDeployments
Content-type: application/json
Content-length: 1892

{
  "@odata.type": "#microsoft.graph.zebraFotaDeployment",
  "displayName": "Display Name value",
  "description": "Description value",
  "deploymentSettings": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentSettings",
    "deviceModel": "Device Model value",
    "updateType": "latest",
    "timeZoneOffsetInMinutes": 7,
    "firmwareTargetBoardSupportPackageVersion": "Firmware Target Board Support Package Version value",
    "firmwareTargetPatch": "Firmware Target Patch value",
    "firmwareTargetOsVersion": "Firmware Target Os Version value",
    "scheduleMode": "scheduled",
    "scheduleDurationInDays": 6,
    "downloadRuleNetworkType": "wifi",
    "downloadRuleStartDateTime": "2016-12-31T23:59:33.2519835-08:00",
    "installRuleStartDateTime": "2017-01-01T00:02:31.1558076-08:00",
    "installRuleWindowStartTime": "11:57:19.2230000",
    "installRuleWindowEndTime": "11:58:38.5330000",
    "batteryRuleMinimumBatteryLevelPercentage": 8,
    "batteryRuleRequireCharger": true
  },
  "deploymentAssignments": [
    {
      "@odata.type": "microsoft.graph.androidFotaDeploymentAssignment",
      "id": "Id value",
      "target": {
        "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget",
        "groupId": "Group Id value"
      }
    }
  ],
  "deploymentStatus": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentStatus",
    "state": "createFailed",
    "totalDevices": 12,
    "totalCreated": 12,
    "totalScheduled": 14,
    "totalDownloading": 0,
    "totalAwaitingInstall": 4,
    "totalSucceededInstall": 5,
    "totalCanceled": 13,
    "totalUnknown": 12,
    "totalFailedDownload": 3,
    "totalFailedInstall": 2,
    "completeOrCanceledDateTime": "2016-12-31T23:59:29.651377-08:00",
    "cancelRequested": true,
    "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
  }
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1941

{
  "@odata.type": "#microsoft.graph.zebraFotaDeployment",
  "id": "8bbfa8a0-a8a0-8bbf-a0a8-bf8ba0a8bf8b",
  "displayName": "Display Name value",
  "description": "Description value",
  "deploymentSettings": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentSettings",
    "deviceModel": "Device Model value",
    "updateType": "latest",
    "timeZoneOffsetInMinutes": 7,
    "firmwareTargetBoardSupportPackageVersion": "Firmware Target Board Support Package Version value",
    "firmwareTargetPatch": "Firmware Target Patch value",
    "firmwareTargetOsVersion": "Firmware Target Os Version value",
    "scheduleMode": "scheduled",
    "scheduleDurationInDays": 6,
    "downloadRuleNetworkType": "wifi",
    "downloadRuleStartDateTime": "2016-12-31T23:59:33.2519835-08:00",
    "installRuleStartDateTime": "2017-01-01T00:02:31.1558076-08:00",
    "installRuleWindowStartTime": "11:57:19.2230000",
    "installRuleWindowEndTime": "11:58:38.5330000",
    "batteryRuleMinimumBatteryLevelPercentage": 8,
    "batteryRuleRequireCharger": true
  },
  "deploymentAssignments": [
    {
      "@odata.type": "microsoft.graph.androidFotaDeploymentAssignment",
      "id": "Id value",
      "target": {
        "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget",
        "groupId": "Group Id value"
      }
    }
  ],
  "deploymentStatus": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentStatus",
    "state": "createFailed",
    "totalDevices": 12,
    "totalCreated": 12,
    "totalScheduled": 14,
    "totalDownloading": 0,
    "totalAwaitingInstall": 4,
    "totalSucceededInstall": 5,
    "totalCanceled": 13,
    "totalUnknown": 12,
    "totalFailedDownload": 3,
    "totalFailedInstall": 2,
    "completeOrCanceledDateTime": "2016-12-31T23:59:29.651377-08:00",
    "cancelRequested": true,
    "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
  }
}
```




