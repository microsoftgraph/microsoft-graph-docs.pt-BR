---
title: Tipo de recurso detectedApp
description: Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado. Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9a234f9a1eeb793bba70c1f091749fae4a589bb5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154856"
---
# <a name="detectedapp-resource-type"></a>Tipo de recurso detectedApp

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado. Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar detectedApps](../api/intune-devices-detectedapp-list.md)|Coleção [detectedApp](../resources/intune-devices-detectedapp.md)|Lista propriedades e relações dos objetos [detectedApp](../resources/intune-devices-detectedapp.md).|
|[Obter detectedApp](../api/intune-devices-detectedapp-get.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|Propriedades de leitura e relações do objeto [detectedApp](../resources/intune-devices-detectedapp.md).|
|[Criar detectedApp](../api/intune-devices-detectedapp-create.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|Cria um novo objeto [detectedApp](../resources/intune-devices-detectedapp.md).|
|[Excluir detectedApp](../api/intune-devices-detectedapp-delete.md)|Nenhum|Exclui um [detectedApp](../resources/intune-devices-detectedapp.md).|
|[Atualizar detectedApp](../api/intune-devices-detectedapp-update.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|Atualiza as propriedades de um objeto [detectedApp](../resources/intune-devices-detectedapp.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do aplicativo detectado. Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado. Somente leitura.|
|displayName|String|Nome do aplicativo descoberto. Somente leitura|
|version|Cadeia de caracteres|Versão do aplicativo descoberto. Somente leitura|
|sizeInByte|Int64|Tamanho do aplicativo descoberto, em bytes. Somente leitura|
|deviceCount|Int32|O número de dispositivos que instalaram esse aplicativo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedDevices|Coleção [managedDevice](../resources/intune-shared-manageddevice.md)|Os dispositivos que descobriram o aplicativo instalado|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```




