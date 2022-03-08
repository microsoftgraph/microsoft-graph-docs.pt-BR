---
title: Tipo de recurso customExtensionHandler
description: Define quando executar uma extensão de fluxo de trabalho de pacote de acesso personalizado.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 59873faa46acb6f258ca6308da2b9d29e323bf65
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337964"
---
# <a name="customextensionhandler-resource-type"></a>Tipo de recurso customExtensionHandler

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define quando executar uma extensão de [fluxo de trabalho de pacote de acesso personalizado](customaccesspackageworkflowextension.md).

Herda da [entidade](entity.md).

## <a name="methods"></a>Métodos
Nenhum.

> [!NOTE]
>
> 1. Para ler os objetos customExtensionHandler em uma política, adição `?$expand=customExtensionHandlers` a uma solicitação [GET accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) . Por exemplo, `GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/4540a08f-8ab5-43f6-a923-015275799197?$expand=customExtensionHandlers`. Para obter mais detalhes, consulte [Exemplo 2: Recuperar os manipuladores de extensão personalizados de uma política](../api/accesspackageassignmentpolicy-get.md#example-2-retrieve-the-custom-extension-handlers-for-a-policy).
>
> 2. Para excluir os **objetos customExtensionHandlers** de uma política, chame [Update accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md) e especifique a propriedade customExtensionHandlers como uma coleção vazia. Para obter mais detalhes, consulte [Exemplo 2: Remover os customExtensionHandlers de uma política](../api/accesspackageassignmentpolicy-update.md#example-2-remove-the-customextensionhandlers-from-a-policy).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String| Identificador do estágio. Herdado da [entidade](../resources/entity.md).|
|stage|accessPackageCustomExtensionStage|Indica o estágio do fluxo de trabalho de solicitação de atribuição de pacote de acesso quando a extensão personalizada do pacote de acesso é executado. Os valores possíveis são `assignmentRequestCreated`, `assignmentRequestApproved`, `assignmentRequestGranted`, `assignmentRequestRemoved`, `assignmentFourteenDaysBeforeExpiration`, `assignmentOneDayBeforeExpiration`, `unknownFutureValue`. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|customExtension|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|Indica qual extensão de fluxo de trabalho personalizada será executada neste estágio. Anulável. Suporta o `$expand`.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customExtensionHandler",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customExtensionHandler",
  "id": "String (identifier)",
  "stage": "String"
}
```

