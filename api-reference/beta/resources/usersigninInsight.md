---
title: Tipo de recurso userSignInInsight
description: Nas análises de acesso do Azure AD, o recurso userSignInInsight representa informações fornecidas aos revisadores com base na última data e hora de entrada do usuário.
author: shubhamguptacal
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ca84ef57b6bb2431210ab3a6a91e80b7089d86bf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112547"
---
# <a name="usersignininsight-resource-type"></a>Tipo de recurso usersignininsight

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa uma visão fornecida aos revisadores com base na última data e hora de login do usuário.

Herda de [governanceInsight](governanceinsight.md).

## <a name="properties"></a>Propriedades
| Propriedade    | Tipo   | Descrição |
| :---------------| :---------- | :---------- |
| lastSignInDateTime | DateTimeOffset | Indica quando o usuário se inscreveu pela última vez |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userSignInInsight",
  "baseType": "microsoft.graph.governanceInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSignInInsight",
  "lastSignInDateTime": "DateTimeOffset"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "usersignininsight resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
