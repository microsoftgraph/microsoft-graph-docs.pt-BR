---
title: Tipo de recurso windowsDefenderApplicationControlSupplementalPolicy
description: Ainda não documentado
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e20f4c9a868d842f5de915f1491d2a9f4428888e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039011"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicy-resource-type"></a>Tipo de recurso windowsDefenderApplicationControlSupplementalPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsDefenderApplicationControlSupplementalPolicies](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-list.md)|[Coleção windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Listar propriedades e relações dos [objetos windowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|
|[Obter windowsDefenderApplicationControlSupplementalPolicy](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-get.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Leia propriedades e relações do [objeto windowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|
|[Criar windowsDefenderApplicationControlSupplementalPolicy](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-create.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Crie um novo [objeto windowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|
|[Excluir windowsDefenderApplicationControlSupplementalPolicy](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-delete.md)|Nenhum|Exclui um [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md).|
|[Atualizar windowsDefenderApplicationControlSupplementalPolicy](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-update.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Atualize as propriedades de um [objeto windowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|
|[atribuir ação](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave para a política suplementar WindowsDefenderApplicationControl.|
|displayName|Cadeia de caracteres|O nome de exibição da política suplementar WindowsDefenderApplicationControl.|
|description|Cadeia de caracteres|A descrição da política suplementar WindowsDefenderApplicationControl.|
|conteúdo|Binário|O conteúdo da política suplementar WindowsDefenderApplicationControl no formato de matriz de byte.|
|contentFileName|Cadeia de Caracteres|O nome do arquivo do conteúdo da política suplementar WindowsDefenderApplicationControl.|
|versão|String|A versão da política suplementar WindowsDefenderApplicationControl.|
|creationDateTime|DateTimeOffset|A data e a hora em que a política suplementar WindowsDefenderApplicationControl foi carregada.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a política suplementar WindowsDefenderApplicationControl foi modificada pela última vez.|
|roleScopeTagIds|String collection|Lista de Marcas de Escopo para esta entidade de política suplementar WindowsDefenderApplicationControl.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[coleção windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|As atribuições de grupo associadas para esta política complementar windowsDefenderApplicationControl.|
|deploySummary|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|Resumo de implantação de política suplementar windowsDefenderApplicationControl.|
|deviceStatuses|[coleção windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)|A lista de estados de implantação de dispositivos para esta política complementar windowsDefenderApplicationControl.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "content": "binary",
  "contentFileName": "String",
  "version": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```



