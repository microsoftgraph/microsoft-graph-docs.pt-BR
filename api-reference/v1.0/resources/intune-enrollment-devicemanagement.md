---
title: Tipo de recurso deviceManagement
description: O recurso deviceManagement representa as identidades de dispositivos da coleção do locatário pré-configuradas no Intune e os perfis de registro que podem ser atribuídos às identidades de dispositivos com suporte para configuração de pré-registro.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 75d859fcb01966a26ccc32f8cea200a18ae65f741cf820ca4f75e858368c21c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230561"
---
# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso deviceManagement representa as identidades de dispositivos da coleção do locatário pré-configuradas no Intune e os perfis de registro que podem ser atribuídos às identidades de dispositivos com suporte para configuração de pré-registro.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune-enrollment-devicemanagement-get.md)|[deviceManagement](../resources/intune-enrollment-devicemanagement.md)|Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-enrollment-devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune-enrollment-devicemanagement-update.md)|[deviceManagement](../resources/intune-enrollment-devicemanagement.md)|Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-enrollment-devicemanagement.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|windowsAutopilotDeviceIdentities|[Coleção windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|As Windows do dispositivo autopilot continham coleção.|
|importedWindowsAutopilotDeviceIdentities|Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Coleção de dispositivos do Windows AutoPilot importados.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




