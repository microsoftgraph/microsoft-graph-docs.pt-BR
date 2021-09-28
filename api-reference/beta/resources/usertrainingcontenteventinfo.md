---
title: Tipo de recurso userTrainingContentEventInfo
description: Representa os detalhes do evento de treinamento dos treinamentos atribuídos aos usuários em uma campanha de simulação e treinamento de ataque.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2771c9924bcd0d3441e404b37f7aa75ec55e9c91
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979492"
---
# <a name="usertrainingcontenteventinfo-resource-type"></a>Tipo de recurso userTrainingContentEventInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes de um evento de treinamento em uma campanha de simulação e treinamento de ataque.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Navegador|Cadeia de Caracteres|Navegador do usuário de onde o evento de treinamento foi gerado.|
|contentDateTime|DateTimeOffset|Data e hora da reprodução de conteúdo de treinamento pelo usuário.|
|ipAddress|Cadeia de caracteres|Endereço IP do usuário para o evento de treinamento.|
|osPlatformDeviceDetails|Cadeia de Caracteres|Os detalhes do sistema operacional, da plataforma e do dispositivo do usuário para o evento de treinamento.|
|potentialScoreImpact|Duplo|Melhoria potencial na postura de segurança do locatário após a conclusão do treinamento pelo usuário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTrainingContentEventInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userTrainingContentEventInfo",
  "contentDateTime": "String (timestamp)",
  "ipAddress": "String",
  "osPlatformDeviceDetails": "String",
  "browser": "String",
  "potentialScoreImpact": "Double"
}
```

