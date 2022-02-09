---
title: Tipo de recurso accessPackageResourceAttributeQuestion
description: Recurso que define a pergunta fornecida a um usuário final, com o objetivo de obter um valor de atributo a ser passado para o sistema final ou para o aprovador de solicitação.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5ced0c1e769000f3624681d92dade18cf8dddcc9
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468276"
---
# <a name="accesspackageresourceattributequestion-resource-type"></a>Tipo de recurso accessPackageResourceAttributeQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recurso que define a [pergunta](accesspackagequestion.md) fornecida a um usuário final, com o objetivo de obter um valor de atributo a ser passado para o sistema final ou para o aprovador de solicitação.

Esse tipo herda de [accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md) e é usado na **propriedade attributeSource** de [um accessPackageResourceAttribute](accesspackageresourceattribute.md).

A única propriedade é **question**, que pode ser [um tipo de objeto accessPackageTextInputQuestion](accesspackagetextinputquestion.md) ou [accessPackageMultipleChoiceQuestion](accesspackagemultiplechoicequestion.md) .

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
