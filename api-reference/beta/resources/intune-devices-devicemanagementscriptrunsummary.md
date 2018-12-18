---
title: tipo de recurso de deviceManagementScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: tfitzmac
ms.openlocfilehash: 347a4e5cd3c4201949841054b69c217ad4f9fa8e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338994"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a>tipo de recurso de deviceManagementScriptRunSummary

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagementScriptRunSummary](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Leia as propriedades e os relacionamentos do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .|
|[Atualizar deviceManagementScriptRunSummary](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Atualize as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave do script de gerenciamento de dispositivo execute entidade resumida.|
|successDeviceCount|Int32|Contagem de sucesso do dispositivo.|
|errorDeviceCount|Int32|Contagem de erros de dispositivo.|
|successUserCount|Int32|Contagem de usuário de sucesso.|
|errorUserCount|Int32|Contagem de erros de usuário.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```





