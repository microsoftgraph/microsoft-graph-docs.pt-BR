---
title: tipo de recurso accessPackageMultipleChoiceQuestion
description: Subclasse de accessPackageQuestion com múltipla escolha como o formato de resposta da pergunta
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ab61a8df1faf0f9b1d9fa3dee10521001ddc6d31
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720069"
---
# <a name="accesspackagemultiplechoicequestion-resource-type"></a>tipo de recurso accessPackageMultipleChoiceQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um filho de **accessPackageQuestion** que apresenta várias opções para as quais o solicitante deve escolher uma resposta.

Herda de [accessPackageQuestion](../resources/accesspackagequestion.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowsMultipleSelection|Booliano|Indica se o solicitante pode selecionar várias opções como resposta.|
|respostas|coleção [accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md)|Lista de opções de resposta.|
|id|Cadeia de caracteres|ID da pergunta. Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).|
|isRequired|Booliano|Indica se o solicitante é necessário para fornecer uma resposta ou não. Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).|
|sequence|Int32|Posição relativa desta pergunta ao exibir uma lista de perguntas para o solicitante. Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).|
|texto|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|O texto da pergunta para mostrar o solicitante. Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).|

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
