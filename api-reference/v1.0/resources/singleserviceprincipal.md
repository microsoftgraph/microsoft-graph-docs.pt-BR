---
title: tipo complexo singleServicePrincipal
description: Identifica uma entidade de serviço no locatário que será permitida como solicitante, aprovador ou revisor.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aaffcafdf0cc8f33efee350e15d0797ad5cba76e
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242170"
---
# <a name="singleserviceprincipal-complex-type"></a>tipo complexo singleServicePrincipal

Namespace: microsoft.graph

Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição de pacote de acesso. O valor indica que esse subjectSet identifica uma entidade de serviço específica no locatário que será permitida como `@odata.type` `#microsoft.graph.singleServicePrincipal` solicitante, aprovador ou revisor. [](../resources/subjectset.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|Descrição dessa entidade de serviço.|
|servicePrincipalId|Cadeia de caracteres|ID do [servicePrincipal](serviceprincipal.md).|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.singleServicePrincipal",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.singleServicePrincipal",
  "servicePrincipalId": "String",
  "description": "String"
}
```



