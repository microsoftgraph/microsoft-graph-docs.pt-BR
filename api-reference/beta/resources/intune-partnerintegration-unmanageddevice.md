---
title: Tipo de recurso unmanagedDevice
description: Dispositivo nãomanageado descoberto na rede.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1606ba0aaedc46ea9a27f6d7d8a0565480c59a01
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59100971"
---
# <a name="unmanageddevice-resource-type"></a>Tipo de recurso unmanagedDevice

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Dispositivo nãomanageado descoberto na rede.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|os|Cadeia de Caracteres|Sistema Operacional.|
|osVersion|String|Versão do sistema operacional.|
|ipAddress|Cadeia de caracteres|Endereço IP.|
|deviceName|Cadeia de caracteres|Nome do dispositivo.|
|macAddress|Cadeia de Caracteres|Endereço MAC.|
|domínio|Cadeia de Caracteres|Domínio.|
|fabricante|String|Fabricante.|
|modelo|String|Modelo.|
|location|Cadeia de Caracteres|Local.|
|lastLoggedOnUser|Cadeia de Caracteres|Último usuário conectado.|
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



