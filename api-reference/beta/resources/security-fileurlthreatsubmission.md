---
title: Tipo de recurso fileUrlThreatSubmission
description: Representa o objeto de envio de ameaças de arquivo criado quando um envio é feito usando uma URL de arquivo.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: b77f0fd8e8fb962546cd473bd3159ae7901c054c
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856563"
---
# <a name="fileurlthreatsubmission-resource-type"></a>Tipo de recurso fileUrlThreatSubmission

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto de envio de ameaça de arquivo criado quando um envio é feito usando uma URL de arquivo. Essa API é reservada e não tem suporte no momento.

Herda de [fileThreatSubmission](../resources/security-filethreatsubmission.md).

## <a name="properties"></a>Propriedades
| Propriedade | Tipo   | Descrição                   |
|:---------|:-------|:------------------------------|
| fileUrl  | Cadeia de caracteres | Especifica a URL do arquivo que precisa ser enviado. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.fileUrlThreatSubmission",
  "baseType": "microsoft.graph.security.fileThreatSubmission",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.fileUrlThreatSubmission",
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
  "fileUrl": "String"
}
```

