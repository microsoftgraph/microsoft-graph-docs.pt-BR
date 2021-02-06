---
title: Tipo de recurso defaultUserRolePermissions
description: Contém determinadas permissões personalizáveis da função de usuário padrão.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b6ee2e8deccf73929b68079379efb0f6d93a3369
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135664"
---
# <a name="defaultuserrolepermissions-resource-type"></a>Tipo de recurso defaultUserRolePermissions

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém determinadas permissões personalizáveis da função de usuário padrão no Azure AD.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| allowedToCreateApps | Boolean | Indica se a função de usuário padrão pode criar aplicativos. |  
| allowedToCreateSecurityGroups | Boolean | Indica se a função de usuário padrão pode criar grupos de segurança. |  
| allowedToReadOtherUsers | Boolean | Indica se a função de usuário padrão pode ler outros usuários. |  

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultUserRolePermissions"
}-->

```json
{
  "allowedToCreateApps": true,
  "allowedToCreateSecurityGroups": true,
  "allowedToReadOtherUsers": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "defaultUserRolePermissions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


