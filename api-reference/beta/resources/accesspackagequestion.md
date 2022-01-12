---
title: Tipo de recurso accessPackageQuestion
description: O tipo complexo para perguntas configuradas em uma política de atribuição de pacote de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: df4158f7869407772b0c7a8807366d03e2ef7a62
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791942"
---
# <a name="accesspackagequestion-resource-type"></a>Tipo de recurso accessPackageQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para a `accessPackageQuestion` propriedade de uma política de atribuição de pacote de [acesso.](accesspackageassignmentpolicy.md) 

Os subtipos [incluem accessPackageTextInputQuestions](accesspackagetextinputquestion.md) [e accessPackageMultipleChoiceQuestions](accesspackagemultiplechoicequestion.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String| ID da pergunta.|
|isRequired|Booliano| Se o solicitante é necessário para fornecer uma resposta ou não.|
|sequence|Int32| Posição relativa dessa pergunta ao exibir uma lista de perguntas para o solicitante.|
|texto|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|O texto da pergunta a ser mostrar ao solicitante.|
|isAnswerEditable|Booliano| Especifica se o solicitante tem permissão para editar respostas a perguntas.|

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