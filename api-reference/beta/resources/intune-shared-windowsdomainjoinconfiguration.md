---
title: tipo de recurso windowsDomainJoinConfiguration
description: Configuração de dispositivo ingresso no domínio do Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b0c133a3729098c028139a525c1ae4bdd2b6b75
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152763"
---
# <a name="windowsdomainjoinconfiguration-resource-type"></a>tipo de recurso windowsDomainJoinConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração de dispositivo ingresso no domínio do Windows.

Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsDomainJoinConfigurations](../api/intune-shared-windowsdomainjoinconfiguration-list.md)|coleção [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|Listar Propriedades e relações dos objetos [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .|
|[Obter windowsDomainJoinConfiguration](../api/intune-shared-windowsdomainjoinconfiguration-get.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|Leia as propriedades e as relações do objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .|
|[Criar windowsDomainJoinConfiguration](../api/intune-shared-windowsdomainjoinconfiguration-create.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|Criar um novo objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .|
|[Excluir windowsDomainJoinConfiguration](../api/intune-shared-windowsdomainjoinconfiguration-delete.md)|Nenhum|Exclui [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).|Excluir um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .|
|[Atualizar windowsDomainJoinConfiguration](../api/intune-shared-windowsdomainjoinconfiguration-update.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|Atualiza as propriedades de um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|**Configuração do dispositivo**|
|activeDirectoryDomainName|String|Nome de domínio do Active Directory para ingressar.|
|computerNameStaticPrefix|String|Prefixo fixo a ser usado para o nome do computador.|
|computerNameSuffixRandomCharCount|Int32|Caracteres gerados dinamicamente usados como sufixo para o nome do computador. Valores válidos de 3 a 14|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|organizationalUnit|String|Unidade organizacional (UO) em que a conta de computador será criada. Se esse parâmetro for NULL, o contêiner do objeto de computador conhecido será usado como publicado no domínio.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Configuração do dispositivo**|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|networkAccessConfigurations|Coleção [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|Referência a configurações de dispositivo necessárias para conectividade de rede|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status da instalação da configuração do dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.  Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão. Objetos Response conterá as propriedades relevantes para o contexto da chamada.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDomainJoinConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "computerNameStaticPrefix": "String",
  "computerNameSuffixRandomCharCount": 1024,
  "activeDirectoryDomainName": "String"
}
```



