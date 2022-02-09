---
title: Tipo de recurso accessPackageMultipleChoiceQuestion
description: Subclasse de accessPackageQuestion que tem várias opções como o formato de resposta da pergunta
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1efcfabbbc345f5820ddaf90bcec9ba9c7076837
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468318"
---
# <a name="accesspackagemultiplechoicequestion-resource-type"></a>Tipo de recurso accessPackageMultipleChoiceQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um filho de **accessPackageQuestion** que apresenta várias opções das quais o solicitante deve escolher uma resposta. Isso é usado na propriedade **questions** de [um accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) e dentro de [um accessPackageResourceAttribute de](accesspackageresourceattribute.md) um recurso de pacote de acesso.

Herda de [accessPackageQuestion](../resources/accesspackagequestion.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowsMultipleSelection|Boolean|Indica se o solicitante pode selecionar várias opções como resposta.|
|choices|[Coleção accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md)|Lista de opções de resposta.|
|id|Cadeia de caracteres|ID da pergunta. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|
|isRequired|Booliano|Indica se o solicitante é necessário para fornecer uma resposta ou não. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|
|sequence|Int32|Posição relativa dessa pergunta ao exibir uma lista de perguntas para o solicitante. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|
|texto|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|O texto da pergunta para mostrar o solicitante. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageMultipleChoiceQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "choices": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
    }
  ],
  "allowsMultipleSelection": "Boolean"
}
```
