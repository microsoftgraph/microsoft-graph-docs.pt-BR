---
title: Tipo de recurso hardwareConfiguration
description: O Intune fornecerá ao cliente a capacidade de configurar configurações de hardware/bios nos dispositivos inscritos do Windows 10 Azure Active Directory ingressados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 895ee4740b588c96fbd10c1b62821ab68e29b54d
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290942"
---
# <a name="hardwareconfiguration-resource-type"></a>Tipo de recurso hardwareConfiguration

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O Intune fornecerá ao cliente a capacidade de configurar configurações de hardware/bios nos dispositivos inscritos do Windows 10 Azure Active Directory ingressados.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar hardwareConfigurations](../api/intune-deviceconfig-hardwareconfiguration-list.md)|[Coleção hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|Listar propriedades e relações dos objetos [hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) .|
|[Obter hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-get.md)|[hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|Leia propriedades e relações do [objeto hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) .|
|[Criar hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-create.md)|[hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|Crie um novo [objeto hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) .|
|[Excluir hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-delete.md)|Nenhuma|Exclui um [hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md).|
|[Atualizar hardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-update.md)|[hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md)|Atualize as propriedades de um [objeto hardwareConfiguration](../resources/intune-deviceconfig-hardwareconfiguration.md) .|
|[ação assignHardwareConfiguration](../api/intune-deviceconfig-hardwareconfiguration-assignhardwareconfiguration.md)|[Coleção hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Ainda não documentado|
|[atribuir ação](../api/intune-deviceconfig-hardwareconfiguration-assign.md)|[Coleção hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para a configuração de hardware|
|versão|Int32|Versão da configuração de hardware (por exemplo. 1, 2, 3 ...)|
|displayName|Cadeia de caracteres|Nome da configuração de hardware|
|description|Cadeia de caracteres|Descrição da configuração de hardware|
|createdDateTime|DateTimeOffset|Data e hora de quando a configuração de hardware foi criada. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Data e hora de quando a configuração de hardware foi modificada. Essa propriedade é somente leitura.|
|fileName|String|Nome do arquivo da configuração de hardware|
|configurationFileContent|Binária|Conteúdo do arquivo da configuração de hardware|
|hardwareConfigurationFormat|[hardwareConfigurationFormat](../resources/intune-deviceconfig-hardwareconfigurationformat.md)|Tipo de oem da configuração de hardware (por exemplo. DELL, HP, Surface e SurfaceDock). Os valores possíveis são: `dell`, `surface`, `surfaceDock`.|
|roleScopeTagIds|String collection|Lista de IDs de marca de escopo para a configuração de hardware|
|perDevicePasswordDisabled|Booliano|Um valor que indica se por pasword devcive desabilitado|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Lista das IDs do grupo de usuários do Azure AD às que a configuração de hardware será aplicada. Somente grupos de segurança e Office 365 grupos são suportados.|
|runSummary|[hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|Um resumo dos resultados de uma tentativa de configurar configurações de hardware|
|deviceRunStates|[Coleção hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Lista de estados de execução para a configuração de hardware em todos os dispositivos|
|userRunStates|[Coleção hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|Lista de estados de execução para a configuração de hardware em todos os usuários|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfiguration",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "fileName": "String",
  "configurationFileContent": "binary",
  "hardwareConfigurationFormat": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "perDevicePasswordDisabled": true
}
```




