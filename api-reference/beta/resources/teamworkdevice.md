---
title: Tipo de recurso teamworkDevice
description: Representa detalhes sobre um Microsoft Teams habilitado para Microsoft Teams que é provisionado para o locatário.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 38058cf2c1697a158eb31c356e22c20af9054156
ms.sourcegitcommit: dab085b74666e190974a35e6a124d3ff1645fa25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2022
ms.locfileid: "64646568"
---
# <a name="teamworkdevice-resource-type"></a>Tipo de recurso teamworkDevice

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes sobre um Microsoft Teams habilitado para Microsoft Teams que é provisionado para o locatário.

Microsoft Teams habilitados para Teams de colaboração certificados. Eles incluem Salas do Microsoft Teams (em Windows e Android), Microsoft Teams telefones, painéis, Surface Hubs e dispositivos SIP. Essas categorias são as mesmas que as disponíveis no centro de administração Teams na seção Teams **dispositivos**.

Para obter mais detalhes, consulte [Manage your devices in Microsoft Teams.](/microsoftteams/devices/device-management)
>**Observação**: isso não inclui telefones celulares, laptops, computadores, guias e assim por diante.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar trabalho em equipeDevices](../api/teamworkdevice-list.md)|Coleção [teamworkDevice](../resources/teamworkdevice.md)|Obter uma lista de todos os Microsoft Teams habilitados para um locatário.|
|[Obter trabalho em equipeDevice](../api/teamworkdevice-get.md)|[teamworkDevice](../resources/teamworkdevice.md)|Obter as propriedades de um dispositivo Microsoft Teams habilitado para uso.|
|[restart](../api/teamworkdevice-restart.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|Reinicie o dispositivo Microsoft Teams habilitado para uso.|
|[runDiagnostics](../api/teamworkdevice-rundiagnostics.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|Execute e gere logs de diagnóstico para o dispositivo Microsoft Teams habilitado para uso.|
|[updateSoftware](../api/teamworkdevice-updatesoftware.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|Atualize o software para um Microsoft Teams habilitado para uso.|
|[Listar operações](../api/teamworkdeviceoperation-list.md)|[Coleção teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|Obter uma lista de operações que estão sendo executados em um dispositivo Teams habilitado para uso.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|activityState|teamworkDeviceActivityState|O estado de atividade do dispositivo. Os valores possíveis são: `unknown`, `busy`, `idle`, `unavailable`, `unknownFutureValue`.|
|companyAssetTag|Cadeia de caracteres|A marca de ativo da empresa atribuída pelo administrador no dispositivo.|
|createdBy|[identitySet](../resources/identityset.md)|Identidade do usuário que registrou o dispositivo no locatário.|
|createdDateTime|DateTimeOffset|A data e a hora UTC em que o dispositivo foi inscrito no locatário.|
|currentUser|[teamworkUserIdentity](../resources/teamworkuseridentity.md)|O usuário conectado no dispositivo.|
|deviceType|[teamworkDeviceType](../resources/teamworkdevice.md#teamworkdevicetype-values)|O tipo de dispositivo. Os valores possíveis são: , , , , `surfaceHub`, `collaborationBar`, `teamsDisplay`, `touchConsole`, `lowCostPhone`, , `teamsPanel`, `sip`, `unknownFutureValue`. `teamsRoom``ipPhone``unknown`|
|hardwareDetail|[teamworkHardwareDetail](../resources/teamworkhardwaredetail.md)|Uma coleção de propriedades relacionadas ao hardware. Por exemplo, **oemSerialNumber e** **model**.|
|healthStatus|[teamworkDeviceHealthStatus](../resources/teamworkdevice.md#teamworkdevicehealthstatus-values)|O status de saúde do dispositivo. Os valores possíveis são: `unknown`, `offline`, `critical`, `nonUrgent`, `healthy`, `unknownFutureValue`.|
|id|String|Identificador de dispositivo. Herdado da [entidade](../resources/entity.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Identidade do usuário que modificou os detalhes do dispositivo pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora UTC em que o detalhe do dispositivo foi modificado pela última vez.|
|notes|String|As anotações adicionadas pelo administrador ao dispositivo.|


### <a name="teamworkdevicetype-values"></a>valores de teamworkDeviceType

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|desconhecido|0|Dispositivo desconhecido.|
|ipPhone|1|Os Telefone IP são os telefones de mesa para que os usuários façam e recebam chamadas de áudio ou participem de reuniões.|
|teamsRoom|2|Salas do Microsoft Teams são Windows dispositivos baseados em IoT projetados para estender a experiência de reunião para a sala de conferência.|
|surfaceHub|3|Surface Hub dispositivos são dispositivos montados na parede ou com suporte para rolos com quadro de comunicação interativo.|
|collaborationBar|4|As barras de colaboração Salas do Microsoft Teams no Android usadas para espaços de reunião pequenos.|
|teamsDisplay|5|Teams dispositivos de exibição são a evolução de Teams telefones. Esses dispositivos são uma categoria de dispositivos de Teams exclusivos que apresentam uma tela sensível ao toque ambiente e uma experiência prática com Cortana.|
|touchConsole|6 |Os dispositivos de console por toque são os periféricos opcionais para o Salas do Teams no Android para executar todas as operações do dispositivo.|
|lowCostPhone|7 |Dispositivos de telefone de baixo custo são telefones Microsoft Teams econômicos.|
|teamsPanel|8 |Microsoft Teams painéis são os dispositivos touchscreen compactos que exibem os detalhes da reunião agendados por meio Teams.|
|sip|9 |Dispositivos SIP (Session Initiation Protocol) que suportam Teams chamadas com o Gateway SIP da Microsoft.|
|unknownFutureValue|10 |Valor de sentinela de enumeração evolvável. Não usar.|


### <a name="teamworkdevicehealthstatus-values"></a>valores de teamworkDeviceHealthStatus

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|desconhecido|0|Status de saúde desconhecido.|
|offline|1|O dispositivo está offline e não pode ser usado.|
|critical|2|O estado exige atenção e ação urgentes, pois pode ter um impacto significativo no desempenho do dispositivo ou torná-lo inutilizável para chamadas ou reuniões.|
|nonUrgent|3|O estado exige atenção devido a problemas ou notificações que podem ter um impacto mínimo no desempenho de um dispositivo online.|
|healthy|4|O dispositivo está online e em boas condições.|
|unknownFutureValue|5|Valor de sentinela de enumeração evolvável. Não usar.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|atividade|[teamworkDeviceActivity](../resources/teamworkdeviceactivity.md)|As propriedades de atividade que mudam com base no uso do dispositivo.|
|configuração|[teamworkDeviceConfiguration](../resources/teamworkdeviceconfiguration.md)|As propriedades de configuração do dispositivo.|
|health|[teamworkDeviceHealth](../resources/teamworkdevicehealth.md)|As propriedades de saúde do dispositivo.|
|operations|[Coleção teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|As operações assíncronas no dispositivo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDevice",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDevice",
  "activityState": "String",
  "companyAssetTag": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "currentUser": {
    "@odata.type": "microsoft.graph.teamworkUserIdentity"
  },
  "deviceType": "String",
  "hardwareDetail": {
    "@odata.type": "microsoft.graph.teamworkHardwareDetail"
  },
  "healthStatus": "String",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "notes": "String"
}
```

