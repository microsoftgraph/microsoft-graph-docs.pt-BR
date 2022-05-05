---
title: Tipo de recurso defaultUserRolePermissions
description: Contém determinadas permissões personalizáveis da função de usuário padrão.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 71edaa99eedc7a37abe5694ace6e5c3c05e29884
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202326"
---
# <a name="defaultuserrolepermissions-resource-type"></a>Tipo de recurso defaultUserRolePermissions

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém determinadas permissões personalizáveis da função de usuário padrão no Azure AD.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| allowedToCreateApps | Booliano | Indica se a função de usuário padrão pode criar aplicativos. |  
| allowedToCreateSecurityGroups | Booliano | Indica se a função de usuário padrão pode criar grupos de segurança. |  
| allowedToReadBitlockerKeysForOwnedDevice | Booliano | Indica se os proprietários registrados de um dispositivo podem ler suas próprias chaves de recuperação do BitLocker com a função de usuário padrão. |
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
  "allowedToReadBitlockerKeysForOwnedDevice": true,
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


