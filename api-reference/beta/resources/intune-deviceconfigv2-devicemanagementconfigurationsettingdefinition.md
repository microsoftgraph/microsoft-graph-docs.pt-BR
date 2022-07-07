---
title: Tipo de recurso deviceManagementConfigurationSettingDefinition
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 206b243c45936efa289024d26051edacc41a2171
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667870"
---
# <a name="devicemanagementconfigurationsettingdefinition-resource-type"></a>Tipo de recurso deviceManagementConfigurationSettingDefinition

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementConfigurationSettingDefinitions](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-list.md)|[Coleção deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Listar propriedades e relações dos [objetos deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .|
|[Obter deviceManagementConfigurationSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-get.md)|[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Ler propriedades e relações do [objeto deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .|
|[Criar deviceManagementConfigurationSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-create.md)|[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Crie um novo [objeto deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .|
|[Excluir deviceManagementConfigurationSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-delete.md)|Nenhum|Exclui um [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).|
|[Atualizar deviceManagementConfigurationSettingDefinition](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition-update.md)|[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Atualize as propriedades de [um objeto deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Aplicabilidade|[deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|Detalhes em qual configuração de dispositivo é aplicável|
|Accesstypes|[deviceManagementConfigurationSettingAccessTypes](../resources/intune-shared-devicemanagementconfigurationsettingaccesstypes.md)|Modo de acesso de leitura/gravação da configuração. Os valores possíveis são: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.|
|palavras-chave|Coleção de cadeias de caracteres|Tokens em que as configurações de pesquisa devem ser pesquisadas|
|infoUrls|String collection|Lista de links em que mais informações sobre a configuração podem ser encontradas em|
|Ocorrência|[deviceManagementConfigurationSettingOccurrence](../resources/intune-shared-devicemanagementconfigurationsettingoccurrence.md)|Indica se a configuração é necessária ou não|
|Baseuri|Cadeia de caracteres|Caminho base do CSP|
|offsetUri|Cadeia de caracteres|Deslocamento do caminho do CSP da Base|
|rootDefinitionId|Cadeia de caracteres|Definição de configuração raiz se a configuração for uma configuração filho.|
|Categoryid|Cadeia de caracteres|Especifica o grupo de áreas no qual a configuração é definida em um CSP (provedor de serviços de configuração) especificado|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-shared-devicemanagementconfigurationsettingusage.md)|Tipo de configuração, por exemplo, configuração e conformidade. Os valores possíveis são: `none`, `configuration`, `compliance`.|
|uxBehavior|[deviceManagementConfigurationControlType](../resources/intune-shared-devicemanagementconfigurationcontroltype.md)|Definindo a representação de tipo de controle na experiência do usuário. Os valores possíveis são: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.|
|visibility|[deviceManagementConfigurationSettingVisibility](../resources/intune-shared-devicemanagementconfigurationsettingvisibility.md)|Definindo o escopo de visibilidade como UX. Os valores possíveis são: `none`, `settingsCatalog`, `template`.|
|referredSettingInformationList|[Coleção deviceManagementConfigurationReferredSettingInformation](../resources/intune-shared-devicemanagementconfigurationreferredsettinginformation.md)|Lista de informações de configuração referenciadas.|
|id|Cadeia de caracteres|Identificador do item|
|descrição|String|Descrição do item|
|Helptext|String|Texto de ajuda do item|
|nome|Cadeia de caracteres|Nome do item|
|displayName|String|Nome de exibição do item|
|versão|String|Versão do Item|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "String",
    "platform": "String",
    "deviceMode": "String",
    "technologies": "String"
  },
  "accessTypes": "String",
  "keywords": [
    "String"
  ],
  "infoUrls": [
    "String"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 1024,
    "maxDeviceOccurrence": 1024
  },
  "baseUri": "String",
  "offsetUri": "String",
  "rootDefinitionId": "String",
  "categoryId": "String",
  "settingUsage": "String",
  "uxBehavior": "String",
  "visibility": "String",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "String"
    }
  ],
  "id": "String (identifier)",
  "description": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String",
  "version": "String"
}
```




