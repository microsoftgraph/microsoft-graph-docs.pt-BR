---
title: Tipo de recurso cloudPC
description: Áreas de trabalho virtuais gerenciadas na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c5fc858e29abf7d649b32991d9e30ce64cc0b632
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721611"
---
# <a name="cloudpc-resource-type"></a>Tipo de recurso cloudPC

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma área de trabalho virtual gerenciada pela nuvem.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[Coleção cloudPC](../resources/cloudpc.md)|Listar propriedades e relações dos objetos [cloudPC.](../resources/cloudpc.md)|
|[Obter cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|Leia as propriedades e as relações de um [objeto cloudPC.](../resources/cloudpc.md)|
|[Reprovision](../api/cloudpc-reprovision.md)|Nenhum(a)|Reprovisionar um [objeto cloudPC.](../resources/cloudpc.md)|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para o computador de nuvem. Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição do computador na nuvem.|
|imageDisplayName|Cadeia de caracteres|Nome da imagem do sistema operacional que está no computador de nuvem.|
|managedDeviceId|Cadeia de caracteres|A ID do dispositivo Intune do computador na nuvem.|
|managedDeviceName|String|O nome do dispositivo Intune do computador na nuvem.|
|provisioningPolicyId|Cadeia de caracteres|ID da política de provisionamento do computador na nuvem.|
|servicePlanId|Cadeia de caracteres|ID do plano de serviço do computador na nuvem.|
|servicePlanName|Cadeia de caracteres|O nome do plano de serviço do computador na nuvem.|
|status|[cloudPcStatus](#cloudpcstatus-values)|Status do computador de nuvem. Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Os detalhes do status do computador na nuvem.|
|userPrincipalName|Cadeia de caracteres|O nome principal do usuário (UPN) do usuário atribuído ao computador de nuvem.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do computador na nuvem. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|

### <a name="cloudpcstatus-values"></a>valores cloudPcStatus

|Member|Descrição|
|:---|:---|
|notProvisioned|O Cloud PC não foi provisionado.|
|provisionamento|O provisionamento do computador na nuvem está em andamento.|
|provisionado|O Cloud PC é provisionado e pode ser acessado por usuários finais.|
|atualização|O resize do Cloud PC está em andamento.|
|inGracePeriod|O Cloud PC está no período de carência de uma semana antes de ser desprovisionado.|
|desprovisionamento|O Cloud PC está desprovisionando.|
|failed|A operação no Cloud PC falhou.|

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
