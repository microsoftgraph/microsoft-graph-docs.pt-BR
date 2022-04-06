---
title: Tipo de recurso delegatedAdminAccessContainer
description: Um contêiner de acesso de administrador através do qual as funções de diretório são atribuídas por meio de uma atribuição de acesso.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 0f129195430f51ca3102f38db5730eb36ea4d7a8
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589588"
---
# <a name="delegatedadminaccesscontainer-resource-type"></a>Tipo de recurso delegatedAdminAccessContainer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um contêiner de acesso de administrador através do qual as funções de diretório são atribuídas por meio de uma atribuição de acesso.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accessContainerId|Cadeia de caracteres|O identificador do contêiner de acesso (por exemplo, um grupo de segurança). Para contêineres de acesso "securityGroup", essa deve ser uma ID válida de um grupo de segurança do Azure AD no locatário do parceiro microsoft.|
|accessContainerType|delegatedAdminAccessContainerType|O tipo de contêiner de acesso (por exemplo, grupo de segurança) que receberá uma ou mais funções por meio de uma relação de administrador delegada. Os valores possíveis são: `securityGroup`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.delegatedAdminAccessContainer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminAccessContainer",
  "accessContainerId": "String",
  "accessContainerType": "String"
}
```

