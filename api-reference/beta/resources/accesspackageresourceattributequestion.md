---
title: Tipo de recurso accessPackageResourceAttributeQuestion
description: Recurso que define a pergunta fornecida a um usuário final, com o objetivo de obter um valor de atributo a ser passado para o sistema final ou para o aprovador de solicitação.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a5731575e5368e50699b57da419b357d145f786f
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61865405"
---
# <a name="accesspackageresourceattributequestion-resource-type"></a>Tipo de recurso accessPackageResourceAttributeQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recurso que define a pergunta fornecida a um usuário final, com o objetivo de obter um valor de atributo a ser passado para o sistema final ou para o aprovador de solicitação.

Herda de [accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|question|accessPackageQuestion|A pergunta pergunta para obter o valor do atributo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttributeQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttributeQuestion",
  "question": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  }
}
```
