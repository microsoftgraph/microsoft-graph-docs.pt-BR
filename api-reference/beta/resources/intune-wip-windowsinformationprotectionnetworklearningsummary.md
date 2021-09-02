---
title: Tipo de recurso windowsInformationProtectionNetworkLearningSummary
description: Entidade de resumo de aprendizagem da Rede de Proteção de Informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 807bfb962a044fcc3ec0687a1b75c4c152b2d1bf
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788413"
---
# <a name="windowsinformationprotectionnetworklearningsummary-resource-type"></a>Tipo de recurso windowsInformationProtectionNetworkLearningSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade de resumo de aprendizagem da Rede de Proteção de Informações do Windows

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsInformationProtectionNetworkLearningSummaries](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-list.md)|Conjunto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Listar propriedades e relações de objetos de [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|
|[Obter windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-get.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Ler propriedades e relações de objetos de [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|
|[Criar windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-create.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Criar um novo objeto de [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|
|[Excluir windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-delete.md)|Nenhum|Excluir [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|
|[Atualizar windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-update.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Atualizar as propriedades de um objeto de [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.|
|url|Cadeia de caracteres|Url do site|
|deviceCount|Int32|Contagem de dispositivos|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionNetworkLearningSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "String (identifier)",
  "url": "String",
  "deviceCount": 1024
}
```



