---
title: Tipo de recurso accessPackageAssignmentRequestorSettings
description: Usado para a propriedade requestorSettings de uma política de atribuição de pacote de acesso. Fornece configurações adicionais para selecionar quem pode criar uma solicitação.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d7a60166f60c2c5882872ed011722fbe14257462
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608249"
---
# <a name="accesspackageassignmentrequestorsettings-complex-type"></a>tipo complexo accessPackageAssignmentRequestorSettings

Namespace: microsoft.graph

Usado para as configurações do solicitante de uma política de atribuição [de pacote de acesso](accesspackageassignmentpolicy.md). Fornece configurações adicionais para selecionar quem pode criar uma solicitação para um pacote de acesso nessa política e o que eles podem incluir em sua solicitação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowCustomAssignmentSchedule|Boolean|If `false`, the requestor is not permitted to include a schedule in their request.|
|enableOnBehalfRequestorsToAddAccess|Booliano|If `true`, permite que os solicitadores em nome dos solicitadores criem uma solicitação para adicionar acesso a outra entidade.|
|enableOnBehalfRequestorsToRemoveAccess|Booliano|If `true`, permite que solicitadores em nome dos solicitadores criem uma solicitação para remover o acesso para outra entidade.|
|enableOnBehalfRequestorsToUpdateAccess|Booliano|If `true`, permite que os solicitadores em nome dos solicitadores criem uma solicitação para atualizar o acesso para outra entidade.|
|enableTargetsToSelfAddAccess|Booliano|If `true`, permite que os solicitadores criem uma solicitação para adicionar acesso a si mesmos.|
|enableTargetsToSelfRemoveAccess|Booliano|If `true`, permite que os solicitadores criem uma solicitação para remover seu acesso.|
|enableTargetsToSelfUpdateAccess|Booliano|If `true`, permite que os solicitadores criem uma solicitação para atualizar seu acesso.|
|onBehalfRequestors|[coleção subjectSet](../resources/subjectset.md)|As entidades que podem solicitar em nome de outras pessoas.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequestorSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequestorSettings",
  "enableTargetsToSelfAddAccess": "Boolean",
  "enableTargetsToSelfUpdateAccess": "Boolean",
  "enableTargetsToSelfRemoveAccess": "Boolean",
  "allowCustomAssignmentSchedule": "Boolean",
  "enableOnBehalfRequestorsToAddAccess": "Boolean",
  "enableOnBehalfRequestorsToUpdateAccess": "Boolean",
  "enableOnBehalfRequestorsToRemoveAccess": "Boolean",
  "onBehalfRequestors": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ]
}
```


