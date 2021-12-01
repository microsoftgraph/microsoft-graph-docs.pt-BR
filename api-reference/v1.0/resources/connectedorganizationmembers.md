---
title: tipo complexo connectedOrganizationMembers
description: O tipo connectedOrganizationMembers identifica uma coleção de usuários no locatário que serão permitidos como solicitante, aprovador ou revisor.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: eb5fce001b0a1e202d0b8f7b1a7f294208e812c1
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242257"
---
# <a name="connectedorganizationmembers-complex-type"></a>tipo complexo connectedOrganizationMembers

Namespace: microsoft.graph


Usado nas configurações de solicitação de uma política de atribuição de pacote de acesso. O valor indica que esse tipo identifica uma coleção de usuários, aqueles associados a uma organização conectada, que terão permissão para solicitar `@odata.type` `#microsoft.graph.connectedOrganizationMembers` um pacote de acesso. [](connectedorganization.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|connectedOrganizationId|String|A ID da organização [conectada no](connectedorganization.md) gerenciamento de direitos.|
|description|Cadeia de caracteres|O nome da organização conectada.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.connectedOrganizationMembers",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectedOrganizationMembers",
  "connectedOrganizationId": "String",
  "description": "String"
}
```



