---
title: Tipo de recurso adminReportSettings
description: Representa as configurações de nível de locatário para relatórios do Microsoft 365.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: reports
author: qiwhuang
ms.openlocfilehash: faa1073175ca09ef4aee52ecfe55d92d24409687
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856468"
---
# <a name="adminreportsettings-resource-type"></a>Tipo de recurso adminReportSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de nível de locatário para relatórios do Microsoft 365.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter adminReportSettings](../api/adminreportsettings-get.md)|[adminReportSettings](../resources/adminreportsettings.md)|Obtenha as configurações de nível de locatário para relatórios do Microsoft 365.|
|[Atualizar adminReportSettings](../api/adminreportsettings-update.md)|[adminReportSettings](../resources/adminreportsettings.md)|Atualize as configurações no nível do locatário para relatórios do Microsoft 365.|

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo           | Descrição                                 |
| -------------- | -------------- | ------------------------------------------- |
| displayConcealedNames | Booliano | Se definido como `true`, todos os relatórios ocultarão informações do usuário, como nomes de usuário, grupos e sites. Se `false`, todos os relatórios mostrarão informações identificáveis. Essa propriedade representa uma configuração no Centro de administração do Microsoft 365. Obrigatório. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminReportSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminReportSettings",
  "displayConcealedNames": "Boolean"
}
```
