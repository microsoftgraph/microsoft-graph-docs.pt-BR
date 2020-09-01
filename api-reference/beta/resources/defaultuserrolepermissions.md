---
title: tipo de recurso defaultUserRolePermissions
description: Contém determinadas permissões personalizáveis de função de usuário padrão.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ca90884220f65bca752fcabe2e0ffe37578cdf90
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319659"
---
# <a name="defaultuserrolepermissions-resource-type"></a>tipo de recurso defaultUserRolePermissions

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém determinadas permissões personalizáveis da função de usuário padrão no Azure AD.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| allowedToCreateApps | Booliano | Indica se a função de usuário padrão pode criar aplicativos. |  
| allowedToCreateSecurityGroups | Booliano | Indica se a função de usuário padrão pode criar grupos de segurança. |  
| allowedToReadOtherUsers | Booliano | Indica se a função de usuário padrão pode ler outros usuários. |  

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
