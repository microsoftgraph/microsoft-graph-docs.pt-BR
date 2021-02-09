---
title: Tipo de recurso unmanagedDevice
description: Dispositivo não-manageado descoberto na rede.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0163fb0f3704bee86622574428954b3c3c9f805a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160082"
---
# <a name="unmanageddevice-resource-type"></a>Tipo de recurso unmanagedDevice

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Dispositivo não-manageado descoberto na rede.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|so|String|Sistema operacional.|
|osVersion|String|Versão do sistema operacional.|
|ipAddress|Cadeia de caracteres|Endereço IP.|
|deviceName|Cadeia de caracteres|Nome do dispositivo.|
|macAddress|String|Endereço MAC.|
|domínio|String|Domínio.|
|fabricante|String|Fabricante.|
|modelo|String|Modelo.|
|localização|String|Localização.|
|lastLoggedOnUser|String|Último usuário conectado.|
|lastSeenDateTime|DateTimeOffset|Data e hora vistas pela última vez.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unmanagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unmanagedDevice",
  "os": "String",
  "osVersion": "String",
  "ipAddress": "String",
  "deviceName": "String",
  "macAddress": "String",
  "domain": "String",
  "manufacturer": "String",
  "model": "String",
  "location": "String",
  "lastLoggedOnUser": "String",
  "lastSeenDateTime": "String (timestamp)"
}
```




