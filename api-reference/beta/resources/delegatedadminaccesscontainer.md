---
title: Tipo de recurso delegatedAdminAccessContainer
description: Um contêiner de acesso de administrador por meio do qual as funções de diretório são atribuídas por meio de uma atribuição de acesso.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 330cbb49f1ad78f327b3d00c9b04b16004de2969
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704328"
---
# <a name="delegatedadminaccesscontainer-resource-type"></a>Tipo de recurso delegatedAdminAccessContainer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um contêiner de acesso de administrador por meio do qual as funções de diretório são atribuídas por meio de uma atribuição de acesso.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accessContainerId|Cadeia de caracteres|O identificador do contêiner de acesso (por exemplo, um grupo de segurança). Para contêineres de acesso "securityGroup", essa deve ser uma ID válida de um grupo de segurança do Azure AD no locatário do parceiro da Microsoft.|
|accessContainerType|delegatedAdminAccessContainerType|O tipo de contêiner de acesso (por exemplo, grupo de segurança) que receberá uma ou mais funções por meio de uma relação de administrador delegado. Os valores possíveis são: `securityGroup`, `unknownFutureValue`.|

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

