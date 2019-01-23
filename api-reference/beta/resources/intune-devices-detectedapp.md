---
title: Tipo de recurso detectedApp
description: Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado. Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4cba801689cb5051926a3139574d5a27294090a0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403095"
---
# <a name="detectedapp-resource-type"></a>Tipo de recurso detectedApp

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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
|id|Cadeia de caracteres|O identificador exclusivo do aplicativo detectado. Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado. Somente leitura.|
|displayName|Cadeia de caracteres|Nome do aplicativo descoberto. Somente leitura|
|version|Cadeia de caracteres|Versão do aplicativo descoberto. Somente leitura|
|sizeInByte|Int64|Tamanho do aplicativo descoberto, em bytes. Somente leitura|
|deviceCount|Int32|O número de dispositivos que instalaram esse aplicativo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managedDevices|Coleção [managedDevice](../resources/intune-devices-manageddevice.md)|Os dispositivos que descobriram o aplicativo instalado|

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




