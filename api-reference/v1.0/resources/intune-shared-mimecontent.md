---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: tfitzmac
ms.openlocfilehash: 53776793fdd057ef057118decf2d72bb0b61a042
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307060"
---
# <a name="mimecontent-resource-type"></a>Tipo de recurso mimeContent

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém as propriedades de um conteúdo genérico MIME.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|type|String|Indica o tipo de conteúdo MIME.|
|valor|Binária|A matriz de byte que contém o conteúdo atual.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



