---
title: Tipo de recurso rolePermission
description: Contém o conjunto de ResourceActions que determina as permissões permitidas e não permitidas para cada função.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3fadd331cfb0e8201dcc77abe066d1c2c0b1c2c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010571"
---
# <a name="rolepermission-resource-type"></a>Tipo de recurso rolePermission

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém o conjunto de ResourceActions que determina as permissões permitidas e não permitidas para cada função.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actions|Coleção de cadeias de caracteres|Ações permitidas-preteridas|
|resourceActions|Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)|Ações de recurso que contêm um conjunto de permissões permitidas e não permitidas.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```





