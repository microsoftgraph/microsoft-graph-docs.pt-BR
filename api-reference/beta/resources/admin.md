---
title: tipo de recurso admin
description: Entidade que atua como um contêiner para a funcionalidade do administrador.
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: fbd064916aca2b0b355eadaa90f56bc2186638ce
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60447016"
---
# <a name="admin-resource-type"></a>tipo de recurso admin

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entidade que atua como um contêiner para a funcionalidade do administrador.

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
| serviceAnnouncement | [serviceAnnouncement](serviceannouncement.md) | Um contêiner para recursos de comunicações de serviço. Somente leitura. |
|windows|[microsoft.graph.windowsUpdates.windows](../resources/windowsupdates-windows.md)|Um contêiner para todas as funcionalidades de serviço de implantação do Update for Business Windows Update for Business. Somente leitura.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.admin",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.admin"
}
```

