---
title: tipo de recurso de administrador
description: Entidade que atua como um contêiner para a funcionalidade de administrador.
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ef9b235a175b3304b9354beddc67f59eb3994cf1
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653494"
---
# <a name="admin-resource-type"></a>tipo de recurso de administrador

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entidade que atua como um contêiner para a funcionalidade de administrador.

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
| serviceAnnouncement | [serviceAnnouncement](serviceannouncement.md) | Um contêiner para recursos de comunicação de serviço. Somente leitura. |
| sharepoint |[microsoft.graph.tenantAdmin.sharepoint](../resources/tenantadmin-sharepoint.md)|Um contêiner para recursos administrativos para gerenciar configurações no nível do locatário para SharePoint e OneDrive.|
| windows |[microsoft.graph.windowsUpdates.windows](../resources/windowsupdates-windows.md)|Um contêiner para todas as Windows Update do serviço de implantação para Empresas. Somente leitura.|

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

