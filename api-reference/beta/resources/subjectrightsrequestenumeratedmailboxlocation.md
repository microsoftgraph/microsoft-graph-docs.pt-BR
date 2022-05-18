---
title: Tipo de recurso subjectRightsRequestEnumeratedMailboxLocation
description: Representa as propriedades de uma solicitação de direitos de assunto que define caixas de correio específicas (Exchange caixas de correio e chats individuais ou Microsoft Teams grupo) como um local de pesquisa.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 1edae24833a7e003fa1a498ca3642508e38af6fa
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461638"
---
# <a name="subjectrightsrequestenumeratedmailboxlocation-resource-type"></a>Tipo de recurso subjectRightsRequestEnumeratedMailboxLocation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as propriedades de uma solicitação de direitos de assunto que define caixas de correio específicas (Exchange caixas de correio e chats individuais ou Microsoft Teams grupo) como um local de pesquisa.

Herda de [subjectRightsRequestMailboxLocation](../resources/subjectrightsrequestmailboxlocation.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|upns|Coleção de cadeias de caracteres|Coleção de caixas de correio que devem ser incluídas na pesquisa. Inclui o UPN (nome upn principal) de cada caixa de correio, por exemplo, `Monica.Thompson@contoso.com`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestEnumeratedMailboxLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestEnumeratedMailboxLocation",
  "upns": [
    "String"
  ]
}
```

