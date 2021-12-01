---
title: tipo complexo groupMembers
description: Identifica uma coleção de usuários no locatário que serão permitidos como solicitante, aprovador ou revisor.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 18260b0b94ddc50e60e60f427e0e4f879912758d
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242213"
---
# <a name="groupmembers-complex-type"></a>tipo complexo groupMembers

Namespace: microsoft.graph


Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição de pacote de acesso.
O valor indica que esse tipo identifica uma coleção de usuários no locatário que serão permitidos como solicitante, aprovador ou `@odata.type` revisor, que são membros de um `#microsoft.graph.groupMembers` grupo específico.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|O nome do grupo no Azure AD. Somente leitura. |
|groupId|Cadeia de caracteres|A ID do [grupo](group.md) no Azure AD.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupMembers",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupMembers",
  "groupId": "String",
  "description": "String"
}
```



