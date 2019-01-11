---
title: tipo de recurso de windowsDomainJoinConfiguration
description: Configuração de dispositivo ingressar de domínio do Windows.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53a3eab41ead346329849be5163452eb9287d94a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823167"
---
# <a name="windowsdomainjoinconfiguration-resource-type"></a>tipo de recurso de windowsDomainJoinConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configuração de dispositivo ingressar de domínio do Windows.

Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windowsDomainJoinConfigurations](../api/intune-shared-windowsdomainjoinconfiguration-list.md)|coleção [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .|
|[Obter windowsDomainJoinConfiguration](../api/intune-shared-windowsdomainjoinconfiguration-get.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|Leia as propriedades e os relacionamentos do objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .|
|[Criar windowsDomainJoinConfiguration](../api/intune-shared-windowsdomainjoinconfiguration-create.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|Crie um novo objeto de [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .|
|[Excluir windowsDomainJoinConfiguration](../api/intune-shared-windowsdomainjoinconfiguration-delete.md)|Nenhum|Exclui um [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).|Exclua um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .|
|[Atualizar windowsDomainJoinConfiguration](../api/intune-shared-windowsdomainjoinconfiguration-update.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|Atualize as propriedades de um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|**Configuração do dispositivo**|
|activeDirectoryDomainName|Cadeia de caracteres|Nome de domínio Active Directory para ingressar.|
|computerNameStaticPrefix|Cadeia de caracteres|Fixo prefixo a ser usado para o nome do computador.|
|computerNameSuffixRandomCharCount|Int32|Caracteres gerados dinamicamente usados como o sufixo de nome do computador. Valores válidos 3 e 14|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|organizationalUnit|Cadeia de caracteres|Unidade organizacional (UO) onde a conta de computador será criada. Se esse parâmetro for NULL, será usado o contêiner de objeto de computador bem conhecido como publicado no domínio.|
|roleScopeTagIds|String collection|Lista de escopo marcas para essa instância da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo. Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Configuração do dispositivo**|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|networkAccessConfigurations|Coleção [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|Referência para as configurações de dispositivo necessário para conectividade de rede|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status da instalação da configuração do dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.  Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Objetos de resposta conterá propriedades relevantes para o contexto da chamada.
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



