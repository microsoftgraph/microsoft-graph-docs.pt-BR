---
title: Tipo de recurso cloudPC
description: Áreas de trabalho virtuais gerenciadas na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 57d708c870339a98cc3fff1322968642ba62f4a1
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534471"
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
|[Reprovision](../api/cloudpc-reprovision.md)|Nenhum|Reprovisionar um [objeto cloudPC.](../resources/cloudpc.md)|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para o Cloud PC. Somente leitura.|
|displayName|String|O nome de exibição do computador na nuvem.|
|imageDisplayName|Cadeia de Caracteres|Nome da imagem do sistema operacional que está no cloud pc.|
|managedDeviceId|Cadeia de Caracteres|A ID do dispositivo Intune do cloud pc.|
|managedDeviceName|String|O nome do dispositivo Intune do computador na nuvem.|
|provisioningPolicyId|Cadeia de Caracteres|A ID da política de provisionamento do Cloud PC.|
|provisioningPolicyName|Cadeia de Caracteres|A política de provisionamento aplicada durante o provisionamento de PCs na Nuvem.|
|onPremisesConnectionName|Cadeia de Caracteres|A conexão local que é aplicada durante o provisionamento de PCs na Nuvem.|
|servicePlanId|Cadeia de Caracteres|ID do plano de serviço do Cloud PC.|
|servicePlanName|Cadeia de caracteres|O nome do plano de serviço do Computador na Nuvem.|
|status|[cloudPcStatus](#cloudpcstatus-values)|Status do computador na nuvem. Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Os detalhes do status do computador na nuvem.|
|userPrincipalName|String|O nome principal do usuário (UPN) do usuário atribuído ao Cloud PC.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do computador na nuvem. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|gracePeriodEndDateTime|DateTimeOffset|A data e a hora em que o período de carência termina e o reprovisionamento/desprovisionamento acontece. Obrigatório somente se o status for `inGracePeriod` . O timestamp é mostrado no formato ISO 8601 e tempo universal coordenado (UTC). Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|

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
  "provisioningPolicyName": "String",
  "onPremisesConnectionName": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "gracePeriodEndDateTime": "String (timestamp)"
}
```
