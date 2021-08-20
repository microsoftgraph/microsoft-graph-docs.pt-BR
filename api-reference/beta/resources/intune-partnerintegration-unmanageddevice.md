---
title: Tipo de recurso unmanagedDevice
description: Dispositivo nãomanageado descoberto na rede.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b98dee94642102bc067efd9b6d8c228d329b406a32ed7c6a8742099f0a60934a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206225"
---
# <a name="unmanageddevice-resource-type"></a>Tipo de recurso unmanagedDevice

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Dispositivo nãomanageado descoberto na rede.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|os|Cadeia de caracteres|Sistema Operacional.|
|osVersion|String|Versão do sistema operacional.|
|ipAddress|Cadeia de caracteres|Endereço IP.|
|deviceName|Cadeia de caracteres|Nome do dispositivo.|
|macAddress|Cadeia de caracteres|Endereço MAC.|
|domínio|Cadeia de caracteres|Domínio.|
|fabricante|String|Fabricante.|
|modelo|String|Modelo.|
|localização|Cadeia de caracteres|Local.|
|lastLoggedOnUser|Cadeia de caracteres|Último usuário conectado.|
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




