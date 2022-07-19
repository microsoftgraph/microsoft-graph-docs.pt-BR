---
title: tipo de recurso de administrador
description: Entidade que atua como um contêiner para a funcionalidade de administrador.
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ce20f9d9a15acbf5c27402eb018b4bbc5ad85b97
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856320"
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
| reportSettings |[microsoft.graph.adminReportSettings](../resources/adminreportsettings.md)|Um contêiner para recursos administrativos para gerenciar relatórios.|
| serviceAnnouncement | [serviceAnnouncement](serviceannouncement.md) | Um contêiner para recursos de comunicação de serviço. Somente leitura. |
| sharepoint |[microsoft.graph.tenantAdmin.sharepoint](../resources/tenantadmin-sharepoint.md)|Um contêiner para recursos administrativos para gerenciar configurações no nível do locatário para o SharePoint e o OneDrive.|
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

