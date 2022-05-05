---
title: Tipo de recurso androidFotaDeploymentAssignmentTarget
description: O AAD grupo no qual estamos implantando atualizações de firmware
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1bc95f25abe2f1971573a4b4904b2535420fe9ff
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212984"
---
# <a name="androidfotadeploymentassignmenttarget-resource-type"></a>Tipo de recurso androidFotaDeploymentAssignmentTarget

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O AAD grupo no qual estamos implantando atualizações de firmware

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|groupId|Cadeia de caracteres|AAD ID do Grupo.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidFotaDeploymentAssignmentTarget",
  "groupId": "String"
}
```




