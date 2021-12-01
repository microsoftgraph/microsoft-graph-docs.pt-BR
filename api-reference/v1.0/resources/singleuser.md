---
title: tipo complexo singleUser
description: Identifica um usuário no locatário que será permitido como solicitante, aprovador ou revisor.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9cc5549ef34fb9ee67a3337e0ba40bc38f413469
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242250"
---
# <a name="singleuser-complex-type"></a>tipo complexo singleUser

Namespace: microsoft.graph

Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição de pacote de acesso. O valor indica que esse userSet identifica um usuário específico no locatário que será permitido como  `@odata.type` `#microsoft.graph.singleUser` solicitante, aprovador ou revisor.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|O nome do usuário no Azure AD. Somente leitura. |
|userId|Cadeia de caracteres|A ID do [usuário no](user.md) Azure AD.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.singleUser",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.singleUser",
  "userId": "String",
  "description": "String"
}
```



