---
title: Tipo de recurso accessPackageQuestion
description: O tipo complexo para perguntas configuradas em uma política de atribuição de pacote de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 22e2cb56461830156d76c10f9e136a62dca4d440
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468304"
---
# <a name="accesspackagequestion-resource-type"></a>Tipo de recurso accessPackageQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para a **propriedade accessPackageQuestion** de uma política [de atribuição](accesspackageassignmentpolicy.md) de pacote de acesso e **o accessPackageResourceAttributeQuestion** em [um accessPackageResourceAttribute](accesspackageresourceattribute.md).

Os subtipos [incluem accessPackageTextInputQuestion](accesspackagetextinputquestion.md) [e accessPackageMultipleChoiceQuestion](accesspackagemultiplechoicequestion.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String| ID da pergunta.|
|isRequired|Booliano| Se o solicitante é necessário para fornecer uma resposta ou não.|
|sequence|Int32| Posição relativa dessa pergunta ao exibir uma lista de perguntas para o solicitante.|
|texto|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|O texto da pergunta a ser mostrar ao solicitante.|
|isAnswerEditable|Boolean| Especifica se o solicitante tem permissão para editar respostas a perguntas.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer"
}
```