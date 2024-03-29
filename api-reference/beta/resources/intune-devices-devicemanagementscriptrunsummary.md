---
title: Tipo de recurso deviceManagementScriptRunSummary
description: Contém propriedades para o resumo de executar um script de gerenciamento de dispositivo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a409bff5addf078e14352217b2bb9cdbeab6f74b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125950"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a>Tipo de recurso deviceManagementScriptRunSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o resumo de executar um script de gerenciamento de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagementScriptRunSummary](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Ler propriedades e relações do [objeto deviceManagementScriptRunSummary.](../resources/intune-devices-devicemanagementscriptrunsummary.md)|
|[Atualizar deviceManagementScriptRunSummary](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Atualize as propriedades de [um objeto deviceManagementScriptRunSummary.](../resources/intune-devices-devicemanagementscriptrunsummary.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de resumo de script de gerenciamento de dispositivos. Essa propriedade é somente leitura.|
|successDeviceCount|Int32|Contagem de dispositivos de sucesso.|
|errorDeviceCount|Int32|Contagem de dispositivos de erro.|
|successUserCount|Int32|Contagem de usuários de sucesso.|
|errorUserCount|Int32|Contagem de usuários de erro.|

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



