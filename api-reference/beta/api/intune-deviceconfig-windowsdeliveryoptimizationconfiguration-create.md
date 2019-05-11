---
title: Criar windowsDeliveryOptimizationConfiguration
description: Criar um novo objeto windowsDeliveryOptimizationConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee20e5836a81600b765bc2dca79b81e97e9cab08
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918056"
---
# <a name="create-windowsdeliveryoptimizationconfiguration"></a>Criar windowsDeliveryOptimizationConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto windowsDeliveryOptimizationConfiguration.

A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDeliveryOptimizationConfiguration.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deliveryOptimizationMode|[windowsDeliveryOptimizationMode](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|Especifica o método de download que a otimização de entrega pode usar para gerenciar o consumo de largura de banda de rede para grandes cenários de distribuição de conteúdo. Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.|
|restrictPeerSelectionBy|[deliveryOptimizationRestrictPeerSelectionByOptions](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|Especifica a restrição da seleção de pares por meio da opção selecionada.
A opção 1 (máscara de sub-rede) só se aplica aos modos de otimização de entrega LAN do modo de download (1) e grupo (2). Os valores possíveis são: `notConfigured` e `subnetMask`.|
|groupIdSource|[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|Especifica a restrição da seleção de par para uma fonte específicas.
As opções definidas nesta política se aplicam apenas ao modo de download grupo (2) do modo de otimização de entrega. Se o grupo (2) não estiver definido como modo de download, esta política será ignorada. Para a opção 3-ID de opção DHCP, o cliente consultará a ID de opção de DHCP 234 e usará o valor de GUID retornado como a ID de grupo.|
|bandwidthmode|[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|Especifica o uso de largura de banda em primeiro plano e plano de fundo usando porcentagens, absolutas ou horas.|
|backgroundDownloadFromHttpDelayInSeconds|Int64|Especifica o número de segundos para atrasar uma origem HTTP em um download em segundo plano que tenha permissão para usar ponto a ponto. Valores válidos de 0 a 4294967295|
|foregroundDownloadFromHttpDelayInSeconds|Int64|Especifica o número de segundos para atrasar uma origem HTTP em um download de primeiro plano que tenha permissão para usar ponto a ponto (0-86400). Valores válidos de 0 a 86400
A especificação de 0 define a otimização de entrega para gerenciar essa configuração usando o serviço de nuvem. Valores válidos de 0 a 86400|
|minimumRamAllowedToPeerInGigabytes|Int32|Especifica o tamanho mínimo de RAM em GB para usar o cache de par (1-100000). Valores válidos de 1 a 100000|
|minimumDiskSizeAllowedToPeerInGigabytes|Int32|Especifica o tamanho mínimo do disco em GB para usar o cache de par (1-100000). Valores válidos de 1 a 100000
Valores recomendados: 64 GB a 256 GB. Valores válidos de 1 a 100000|
|minimumFileSizeToCacheInMegabytes|Int32|Especifica o tamanho mínimo do arquivo de conteúdo em MB habilitado para usar o cache de ponto (1-100000). Valores válidos de 1 a 100000
Valores recomendados: 1 MB a 100.000 MB. Valores válidos de 1 a 100000|
|minimumBatteryPercentageAllowedToUpload|Int32|Especifica a porcentagem de bateria mínima para permitir que o dispositivo carregue dados (0-100). Valores válidos de 0 a 100
O valor padrão é 0. O valor 0 (zero) significa "não limitado" e o valor padrão do serviço de nuvem será usado. Valores válidos de 0 a 100|
|modifyCacheLocation|Cadeia de caracteres|Especifica a unidade que a otimização de entrega deve usar para seu cache.|
|maximumCacheAgeInDays|Int32|Especifica o tempo máximo, em dias, em que cada arquivo é mantido no cache de otimização de entrega após o download bem-sucedido (0-49710). Valores válidos de 0 a 49710|
|maximumCacheSize|[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|Especifica o tamanho máximo de cache que a otimização de entrega como uma porcentagem ou em GB.|
|vpnPeerCaching|[habilitação](../resources/intune-shared-enablement.md)|Especifica se o dispositivo tem permissão para participar do cache de mesmo nível enquanto conectado via VPN à rede de domínio. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1060

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1232

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled"
}
```




