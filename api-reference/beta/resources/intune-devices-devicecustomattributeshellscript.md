---
title: Tipo de recurso deviceCustomAttributeShellScript
description: Representa um script de atributo personalizado para macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 32d1e032e8bc781a9f7ab1d433e1c8b757097ca6494c68094addde0812898376
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239403"
---
# <a name="devicecustomattributeshellscript-resource-type"></a>Tipo de recurso deviceCustomAttributeShellScript

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um script de atributo personalizado para macOS.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceCustomAttributeShellScripts](../api/intune-devices-devicecustomattributeshellscript-list.md)|[Coleção deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Listar propriedades e relações dos [objetos deviceCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)|
|[Obter deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-get.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Leia propriedades e relações do [objeto deviceCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)|
|[Criar deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-create.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Crie um novo [objeto deviceCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)|
|[Excluir deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-delete.md)|Nenhum|Exclui um [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md).|
|[Atualizar deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-update.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Atualize as propriedades de [um objeto deviceCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)|
|[atribuir ação](../api/intune-devices-devicecustomattributeshellscript-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da entidade de atributo personalizado.|
|customAttributeName|Cadeia de caracteres|O nome do atributo personalizado.|
|customAttributeType|[deviceCustomAttributeValueType](../resources/intune-devices-devicecustomattributevaluetype.md)|O tipo esperado do valor do atributo personalizado. Os valores possíveis são: `integer`, `string`, `dateTime`.|
|displayName|Cadeia de caracteres|Nome do script de gerenciamento de dispositivos.|
|description|Cadeia de caracteres|Descrição opcional para o script de gerenciamento de dispositivos.|
|scriptContent|Binário|O conteúdo do script.|
|createdDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivos foi criado. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivos foi modificado pela última vez. Essa propriedade é somente leitura.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|fileName|String|Nome do arquivo de script.|
|roleScopeTagIds|String collection|Lista de IDs de marca de escopo para esta instância do PowerShellScript.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|A lista de atribuições de grupo para o script de gerenciamento de dispositivos.|
|assignments|[Coleção deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|A lista de atribuições de grupo para o script de gerenciamento de dispositivos.|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Execute o resumo do script de gerenciamento de dispositivos.|
|deviceRunStates|[Coleção deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Lista de estados de executar para esse script em todos os dispositivos.|
|userRunStates|[Coleção deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Lista de estados de executar para esse script em todos os usuários.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCustomAttributeShellScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCustomAttributeShellScript",
  "id": "String (identifier)",
  "customAttributeName": "String",
  "customAttributeType": "String",
  "displayName": "String",
  "description": "String",
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




