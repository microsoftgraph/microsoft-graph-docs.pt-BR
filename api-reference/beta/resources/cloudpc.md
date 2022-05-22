---
title: Tipo de recurso cloudPC
description: Áreas de trabalho virtuais gerenciadas na nuvem.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: f529b46fc5bb11be7f58fbd4068789d5def4e824
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628849"
---
# <a name="cloudpc-resource-type"></a>Tipo de recurso cloudPC

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma área de trabalho virtual gerenciada pela nuvem. Esse PC na nuvem também é registrado no Intune gerenciado por meio do portal do Microsoft Endpoint Manager, portanto, o PC na nuvem também tem uma ID de dispositivo gerenciado Intune correspondente.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|coleção [cloudPC](../resources/cloudpc.md)|Listar propriedades e relações dos objetos [cloudPC](../resources/cloudpc.md) .|
|[Obter cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|Leia as propriedades e as relações de um [objeto cloudPC](../resources/cloudpc.md) .|
|[Alterar o tipo de conta de usuário](../api/cloudpc-changeuseraccounttype.md)|Nenhum|Altere o tipo de conta do usuário em um PC na nuvem específico.|
|[Fim do período de carência](../api/cloudpc-endgraceperiod.md)|Nenhum|Encerrar o período de carência para um [objeto cloudPC](../resources/cloudpc.md) .|
|[Obter resultados da ação remota](../api/manageddevice-getcloudpcremoteactionresults.md)|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|Verifique os resultados [da ação remota especificada pelo PC na nuvem](../resources/cloudpcremoteactionresult.md) para um dispositivo de PC na nuvem.|
|[Reiniciar](../api/cloudpc-reboot.md)|Nenhum|Reinicialize um objeto [cloudPC](../resources/cloudpc.md) específico.|
|[Rename](../api/cloudpc-rename.md)|Nenhum|Renomeie um objeto [cloudPC](../resources/cloudpc.md) específico. Use essa API para atualizar o **displayName** para a entidade pc na nuvem.|
|[Reprovisionar](../api/cloudpc-reprovision.md)|Nenhum|Reprovisionar um [objeto cloudPC](../resources/cloudpc.md) .|
|[Reprovisionar ação remota](../api/manageddevice-reprovisioncloudpc.md)|Nenhum|Reprovisionar um PC na nuvem com Intune ID [do dispositivo](../resources/cloudpc.md) gerenciado.  |
|[Ação remota de reprovisionamento em massa](../api/manageddevice-bulkreprovisioncloudpc.md)|Nenhum|Reprovisionar em massa um conjunto de dispositivos de PC na nuvem com Intune IDs de dispositivo gerenciado.|
|[Redimensionar ação remota](../api/manageddevice-resizecloudpc.md)|Nenhum|Atualize ou faça downgrade de um PC na nuvem existente para outra configuração com nova vCPU e tamanho de armazenamento por meio Intune ID do dispositivo gerenciado.|
|[Solução de problemas](../api/cloudpc-troubleshoot.md)|Nenhum|Solucionar problemas de um [objeto cloudPC](../resources/cloudpc.md) específico. Use essa API para verificar o status de integridade do PC na nuvem e do host da sessão.|
|[Restaurar ação remota](../api/manageddevice-restorecloudpc.md)|Nenhum|Restaure um dispositivo de PC na nuvem para um estado anterior de um instantâneo.|
|[Ação remota de restauração em massa](../api/manageddevice-bulkrestorecloudpc.md)|[cloudPcBulkRemoteActionResult](../resources/cloudpcbulkremoteactionresult.md)|Restaure vários dispositivos de PC na nuvem com uma única solicitação que inclui as IDs Intune dispositivos gerenciados e uma data e hora do ponto de restauração.|
|[Definir o status da revisão](../api/manageddevice-setcloudpcreviewstatus.md)|Nenhum|Defina o status de revisão de um dispositivo de PC na nuvem específico.|
|[Obter status de revisão](../api/manageddevice-getcloudpcreviewstatus.md)|[cloudPcReviewStatus](../resources/cloudpcreviewstatus.md)|Obter o status de revisão de um dispositivo de PC na nuvem específico.|
|[Status da revisão do conjunto em massa](../api/manageddevice-bulksetcloudpcreviewstatus.md)|[cloudPcBulkRemoteActionResult](../resources/cloudpcbulkremoteactionresult.md)|Defina o status de revisão de vários dispositivos de PC na nuvem com uma única solicitação que inclui as IDs de Intune gerenciados.|
|[Lista de usuários](../api/user-list-cloudpcs.md)|coleção [cloudPC](../resources/cloudpc.md)|Liste os dispositivos [cloudPC](../resources/cloudpc.md) atribuídos ao usuário conectado.|
|[Obter informações de inicialização para o usuário](../api/cloudpc-getcloudpclaunchinfo.md)|[cloudPCLaunchInfo](../resources/cloudpclaunchinfo.md)|Obtenha [o cloudPCLaunchInfo](../resources/cloudpclaunchinfo.md) para o usuário conectado.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aadDeviceId|Cadeia de caracteres|A Azure Active Directory (Azure AD) do computador na nuvem.|
|displayName|Cadeia de caracteres|O nome de exibição do PC na nuvem.|
|gracePeriodEndDateTime|DateTimeOffset|A data e a hora em que o período de carência termina e ocorre o reprovisionamento/desprovisionamento. Obrigatório somente se o status for `inGracePeriod`. O carimbo de data/hora é mostrado no formato ISO 8601 e no UTC (Tempo Universal Coordenado). Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|id|Cadeia de caracteres|O identificador exclusivo para o PC na nuvem. Somente leitura.|
|imageDisplayName|Cadeia de Caracteres|Nome da imagem do sistema operacional que está no PC na nuvem.|
|lastLoginResult|[cloudPcLoginResult](../resources/cloudpcloginresult.md)|O último resultado de logon do PC na nuvem. Por exemplo, `{ "time": "2014-01-01T00:00:00Z"}`.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação do PC na nuvem. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|lastRemoteActionResult|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|O último resultado de ação remota dos PCs na nuvem corporativos. As ações remotas com suporte são: `Reboot`, `Rename`, `Reprovision`, `Restore`e `Troubleshoot`.|
|managedDeviceId|Cadeia de Caracteres|A Intune ID do dispositivo do PC na nuvem.|
|managedDeviceName|String|O Intune do dispositivo do PC na nuvem.|
|onPremisesConnectionName|Cadeia de Caracteres|A conexão de rede do Azure que é aplicada durante o provisionamento de PCs na nuvem.|
|osVersion|[cloudPcOperatingSystem](../resources/cloudpcorganizationsettings.md#cloudpcoperatingsystem-values)|A versão do sistema operacional (SO) a ser provisionada em PCs na nuvem. Os valores possíveis são: `windows10`, `windows11`e `unknownFutureValue`.|
|provisioningPolicyId|Cadeia de caracteres|A ID da política de provisionamento do PC na nuvem.|
|provisioningPolicyName|Cadeia de Caracteres|A política de provisionamento que é aplicada durante o provisionamento de PCs na nuvem.|
|servicePlanId|Cadeia de Caracteres|A ID do plano de serviço do PC na nuvem.|
|servicePlanName|Cadeia de caracteres|O nome do plano de serviço do PC na nuvem.|
|servicePlanType|[cloudPcServicePlanType](../resources/cloudpcserviceplan.md#cloudpcserviceplantype-values)|O tipo de plano de serviço do PC na nuvem.|
|status|[cloudPcStatus](#cloudpcstatus-values)|O status do PC na nuvem. Os valores possíveis são: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`, `restoring`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Os detalhes do status do PC na nuvem.|
|userAccountType|[cloudPcUserAccountType](../resources/cloudpcorganizationsettings.md#cloudpcuseraccounttype-values)|O tipo de conta do usuário em PCs na nuvem provisionados. Os valores possíveis são: `standardUser`, `administrator`e `unknownFutureValue`.|
|userPrincipalName|Cadeia de caracteres|O NOME UPN do usuário atribuído ao PC na nuvem.|

### <a name="cloudpcstatus-values"></a>Valores de cloudPcStatus

|Member|Descrição|
|:---|:---|
|notProvisioned|O PC na nuvem não foi provisionado.|
|Provisionamento|O provisionamento de PC na nuvem está em andamento.|
|provisionado|O PC na nuvem é provisionado e pode ser acessado pelos usuários finais.|
|inGracePeriod|O PC na nuvem está no período de carência de uma semana antes de ser desprovisionado.|
|Desprovisionamento|O PC na nuvem está sendo desprovisionado.|
|Falhou|A operação no PC na nuvem falhou.|
|provisionedWithWarnings|O PC na nuvem é provisionado e pode ser acessado pelos usuários finais, mas com alguns avisos. O usuário pode continuar a usar este PC na nuvem.|
|Redimensionamento|O PC na nuvem está redimensionando.|
|pendingProvision|O provisionamento está pendente no PC na nuvem. Nesse caso, o número de PCs na nuvem no período de carência é maior do que o número total de licenças disponíveis. |
|Restaurar|O PC na nuvem está restaurando.|
|unknownFutureValue|Valor de sentinel de enumeração evolvável. Não usar.|

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
  "aadDeviceId": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "provisioningPolicyId": "String",
  "provisioningPolicyName": "String",
  "onPremisesConnectionName": "String",
  "servicePlanId": "String",
  "servicePlanType": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "gracePeriodEndDateTime": "String (timestamp)",
  "userAccountType": "String",
  "osVersion": "String",
  "lastRemoteActionResult": "String",
  "lastLoginResult": "String"
}
```
