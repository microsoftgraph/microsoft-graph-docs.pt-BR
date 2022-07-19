---
title: Tipo de recurso fileContentThreatSubmission
description: Representa um objeto de envio de ameaça criado quando o envio é feito usando o conteúdo de um arquivo.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 309a7c109fd6db793f91bf04bc77f66e3659d079
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856565"
---
# <a name="filecontentthreatsubmission-resource-type"></a>Tipo de recurso fileContentThreatSubmission

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto de envio de ameaça criado quando o envio é feito usando o conteúdo de um arquivo.

Herda de [fileThreatSubmission](../resources/security-filethreatsubmission.md).

## <a name="properties"></a>Propriedades
| Propriedade    | Tipo   | Descrição                  |
|:------------|:-------|:-----------------------------|
| Filecontent | Cadeia de caracteres | Especifica o conteúdo do arquivo no formato base 64. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.fileContentThreatSubmission",
  "baseType": "microsoft.graph.security.fileThreatSubmission",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.fileContentThreatSubmission",
  "id": "String (identifier)",
  "tenantId": "String",
  "createdDateTime": "String (timestamp)",
  "contentType": "String",
  "category": "String",
  "source": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.security.submissionUserIdentity"
  },
  "status": "String",
  "result": {
    "@odata.type": "microsoft.graph.security.submissionResult"
  },
  "adminReview": {
    "@odata.type": "microsoft.graph.security.submissionAdminReview"
  },
  "clientSource": "String",
  "fileName": "String",
  "fileContent": "String"
}
```

