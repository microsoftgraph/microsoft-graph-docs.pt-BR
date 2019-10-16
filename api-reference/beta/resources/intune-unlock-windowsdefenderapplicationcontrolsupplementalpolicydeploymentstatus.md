---
title: tipo de recurso windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: Contém propriedades para o estado de implantação de uma política suplementar do WindowsDefenderApplicationControl para um dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e10728bba5048b1e46889c178710b79043622624
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538837"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-resource-type"></a>tipo de recurso windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o estado de implantação de uma política suplementar do WindowsDefenderApplicationControl para um dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatuses](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-list.md)|coleção [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Listar Propriedades e relações dos objetos [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .|
|[Obter windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-get.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Leia as propriedades e as relações do objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .|
|[Criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-create.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Criar um novo objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .|
|[Excluir windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-delete.md)|Nenhum|Exclui [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md).|
|[Atualizar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus-update.md)|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|Atualiza as propriedades de um objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|deviceName|Cadeia de caracteres|Nome do dispositivo.|
|deviceId|Cadeia de caracteres|ID de dispositivo.|
|lastSyncDateTime|DateTimeOffset|Hora da data da última sincronização.|
|osVersion|String|Versão do sistema operacional Windows.|
|osDescription|Cadeia de caracteres|Descrição da versão do sistema operacional Windows.|
|deploymentStatus|[windowsDefenderApplicationControlSupplementalPolicyStatuses](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|O estado de implantação da política. Os valores possíveis são: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.|
|userName|Cadeia de caracteres|O nome do usuário deste dispositivo.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário.|
|policyVersion|Cadeia de caracteres|Versão de leitura humana da política complementar do WindowsDefenderApplicationControl.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|política|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|O link de navegação para a política complementar do WindowsDefenderApplicationControl.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "osVersion": "String",
  "osDescription": "String",
  "deploymentStatus": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "policyVersion": "String"
}
```



