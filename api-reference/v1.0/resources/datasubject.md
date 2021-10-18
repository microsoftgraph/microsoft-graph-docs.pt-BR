---
title: Tipo de recurso dataSubject
description: Contém informações relacionadas ao assunto de uma pesquisa de conteúdo.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 10d04fb473da2e704c811a34fcf23800ac6f1665
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60449128"
---
# <a name="datasubject-resource-type"></a>Tipo de recurso dataSubject

Namespace: microsoft.graph

Contém informações relacionadas ao assunto de uma pesquisa de conteúdo. Esse recurso é um tipo aberto e oferece suporte à adição de propriedades de adição; por exemplo, iD do cliente.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|email|Cadeia de caracteres|Email do assunto de dados.|
|firstName|Cadeia de caracteres|Nome do assunto de dados.|
|lastName|Cadeia de caracteres|Sobrenome do assunto de dados.|
|residência|String|O país/região da residência. As informações de residência são fornecidas apenas para relatórios internos, mas não para a pesquisa de conteúdo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dataSubject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSubject",
  "email": "String",
  "firstName": "String",
  "lastName": "String",
  "residency": "String",
  "SSN": "String"
}
```

