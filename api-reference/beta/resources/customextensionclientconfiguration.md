---
title: Tipo de recurso customExtensionClientConfiguration
description: Configurações de conexão HTTP que definem por quanto tempo o Azure AD pode aguardar uma resposta de um aplicativo lógico antes de desligar a conexão. Somente timeoutInMilliseconds é suportado.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2c04e53560aecc3e41978b569e42d993477eca87
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338154"
---
# <a name="customextensionclientconfiguration-resource-type"></a>Tipo de recurso customExtensionClientConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações de conexão HTTP que definem por quanto tempo o Azure AD pode aguardar uma resposta de um aplicativo lógico antes de desligar a conexão. Somente **timeoutInMilliseconds** é suportado.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|timeoutInMilliseconds|Int32|A duração máxima em milissegundos que o Azure AD aguardará por uma resposta do aplicativo lógico antes de desligar a conexão. O intervalo válido é entre `200` e `2000` milissegundos. A duração padrão é `1000`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customExtensionClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customExtensionClientConfiguration",
  "timeoutInMilliseconds": "Integer"
}
```

