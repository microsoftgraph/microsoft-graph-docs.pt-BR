---
title: Tipo de recurso zebraFotaArtifact
description: Descreve um único artefato para um modelo de dispositivo específico.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cea341ecb1d3151e8e4f895f6038b7f47cb95cba
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213046"
---
# <a name="zebrafotaartifact-resource-type"></a>Tipo de recurso zebraFotaArtifact

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve um único artefato para um modelo de dispositivo específico.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar zebraFotaArtifacts](../api/intune-androidfotaservice-zebrafotaartifact-list.md)|[Coleção zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md)|Listar propriedades e relações dos [objetos zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) .|
|[Obter zebraFotaArtifact](../api/intune-androidfotaservice-zebrafotaartifact-get.md)|[zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md)|Ler propriedades e relações do objeto [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) .|
|[Criar zebraFotaArtifact](../api/intune-androidfotaservice-zebrafotaartifact-create.md)|[zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md)|Crie um novo [objeto zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) .|
|[Excluir zebraFotaArtifact](../api/intune-androidfotaservice-zebrafotaartifact-delete.md)|Nenhuma|Exclui um [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md).|
|[Atualizar zebraFotaArtifact](../api/intune-androidfotaservice-zebrafotaartifact-update.md)|[zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md)|Atualize as propriedades de um [objeto zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID de ZebraFotaArtifact.|
|deviceModel|Cadeia de caracteres|Modelo de dispositivo de artefato.|
|osVersion|String|Versão do sistema operacional do artefato.|
|patchVersion|Cadeia de Caracteres|Versão do patch do artefato.|
|boardSupportPackageVersion|Cadeia de Caracteres|A versão do Pacote de Suporte do Board.|
|releaseNotesUrl|Cadeia de Caracteres|URL de notas de versão do artefato.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.zebraFotaArtifact"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaArtifact",
  "id": "String (identifier)",
  "deviceModel": "String",
  "osVersion": "String",
  "patchVersion": "String",
  "boardSupportPackageVersion": "String",
  "releaseNotesUrl": "String"
}
```




