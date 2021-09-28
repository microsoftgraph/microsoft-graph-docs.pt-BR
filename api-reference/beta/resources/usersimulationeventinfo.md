---
title: Tipo de recurso userSimulationEventInfo
description: Representa o evento de simulação de um usuário em um locatário em uma campanha de simulação e treinamento de ataque.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 423eb3f5f15d4730d1229febde71aec9930ff81f
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979450"
---
# <a name="usersimulationeventinfo-resource-type"></a>Tipo de recurso userSimulationEventInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um evento de simulação de um usuário em um locatário em uma campanha de simulação e treinamento de ataque.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Navegador|Cadeia de caracteres|Informações do navegador de onde o evento de simulação foi iniciado por um usuário em uma campanha de simulação e treinamento de ataque.|
|eventDateTime|DateTimeOffset|Data e hora do evento de simulação por um usuário em uma campanha de simulação e treinamento de ataque.|
|eventName|Cadeia de caracteres|Nome do evento de simulação por um usuário em uma campanha de simulação e treinamento de ataque.|
|ipAddress|Cadeia de caracteres|Endereço IP de onde o evento de simulação foi iniciado por um usuário em uma campanha de simulação e treinamento de ataque.|
|osPlatformDeviceDetails|Cadeia de Caracteres|Os detalhes do sistema operacional, plataforma e dispositivo de onde o evento de simulação foi iniciado por um usuário em uma campanha de simulação e treinamento de ataques.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userSimulationEventInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSimulationEventInfo",
  "eventName": "String",
  "eventDateTime": "String (timestamp)",
  "ipAddress": "String",
  "osPlatformDeviceDetails": "String",
  "browser": "String"
}
```

