---
title: tipo de recurso cloudPC
description: Áreas de trabalho virtuais gerenciadas pela nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 95758299f87ac463bac6fdc30f7d70fb59eb6c92
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378255"
---
# <a name="cloudpc-resource-type"></a>tipo de recurso cloudPC

Namespace: microsoft.graph

Representa uma área de trabalho virtual gerenciada em nuvem.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|coleção [cloudPC](../resources/cloudpc.md)|Listar Propriedades e relações dos objetos [cloudPC](../resources/cloudpc.md) .|
|[Obter cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|Leia as propriedades e os relacionamentos de um objeto [cloudPC](../resources/cloudpc.md) .|
|[Reprovisionar](../api/cloudpc-reprovision.md)|Nenhum|Reprovisionar um objeto [cloudPC](../resources/cloudpc.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do PC de nuvem. Somente leitura.|
|displayName|String|O nome de exibição do computador de nuvem.|
|imageDisplayName|Cadeia de Caracteres|Nome da imagem do sistema operacional que está no computador de nuvem.|
|managedDeviceId|Cadeia de Caracteres|A ID de dispositivo do Intune do PC na nuvem.|
|managedDeviceName|String|O nome do dispositivo do Intune no Cloud PC.|
|provisioningPolicyId|Cadeia de Caracteres|A ID da política de provisionamento do PC da nuvem.|
|onplanid|Cadeia de Caracteres|A ID do plano de serviço do computador de nuvem.|
|onplanname|Cadeia de caracteres|O nome do plano de serviço do computador da nuvem.|
|status|cloudPcStatus|Status do PC de nuvem. Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `upgradeFailed`, `provisionFailed`, `deprovisionFailed`, `reprovisionFailed`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Os detalhes do status do PC de nuvem.|
|userPrincipalName|String|O nome principal do usuário (UPN) do usuário atribuído ao computador da nuvem.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora da última modificação do computador da nuvem. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPC",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPC",
  "id": "String (identifier)",
  "displayName": "String",
  "imageDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "provisioningPolicyId": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```
