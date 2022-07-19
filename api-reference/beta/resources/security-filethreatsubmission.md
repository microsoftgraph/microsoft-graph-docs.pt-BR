---
title: Tipo de recurso fileThreatSubmission
description: Representa um envio de ameaças relacionado a um arquivo.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6c592e2f0b5a22cf564a790c6f7934ba766771cd
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856564"
---
# <a name="filethreatsubmission-resource-type"></a>Tipo de recurso fileThreatSubmission

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um envio de ameaças relacionado a um arquivo. Ele é usado para enviar anexos de email de malware suspeitos para Microsoft Defender para Office 365. Ele também pode ser usado para enviar casos falsos positivos que não devem ter sido bloqueados por Microsoft Defender para Office 365, por exemplo, um anexo de email seguro.

Atualmente, o envio de ameaças de arquivo é roteado para Microsoft Defender para Office 365. No futuro, ele pode ser roteado para Microsoft Defender para Ponto de Extremidade. Essa é uma interface unificada para envio de ameaças de arquivo, independentemente de onde ele é roteado.

Esse é um tipo abstrato. Herda de [threatSubmission](../resources/security-threatsubmission.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar fileThreatSubmissions](../api/security-filethreatsubmission-list.md)|[coleção microsoft.graph.security.fileThreatSubmission](../resources/security-filethreatsubmission.md)|Obtenha uma lista dos [objetos fileThreatSubmission](../resources/security-filethreatsubmission.md) e suas propriedades.|
|[Criar fileThreatSubmission](../api/security-filethreatsubmission-post-filethreats.md)|[microsoft.graph.security.fileThreatSubmission](../resources/security-filethreatsubmission.md)|Crie um novo [objeto fileThreatSubmission](../resources/security-filethreatsubmission.md) .|
|[Obter fileThreatSubmission](../api/security-filethreatsubmission-get.md)|[microsoft.graph.security.fileThreatSubmission](../resources/security-filethreatsubmission.md)|Leia as propriedades e as relações de um [objeto fileThreatSubmission](../resources/security-filethreatsubmission.md) .|

## <a name="properties"></a>Propriedades
| Propriedade | Tipo   | Descrição                    |
|:---------|:-------|:-------------------------------|
| fileName | String | Especifica o nome do arquivo a ser enviado. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.fileThreatSubmission",
  "baseType": "microsoft.graph.security.threatSubmission",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.fileThreatSubmission",
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
  "fileName": "String"
}
```

