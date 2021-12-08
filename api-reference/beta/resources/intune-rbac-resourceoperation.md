---
title: Tipo de recurso resourceOperation
description: Descreve o recurso resourceOperation (entidade) da API do Microsoft Graph (REST), que dá suporte a fluxos de trabalho do Intune relacionados ao controle de acesso baseado em função (RBAC).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b70ccf88ab0563620c66b289ed0bcbfdef2b3d2
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340162"
---
# <a name="resourceoperation-resource-type"></a>Tipo de recurso resourceOperation

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve o recurso resourceOperation (entidade) da API do Microsoft Graph (REST), que dá suporte a fluxos de trabalho do Intune relacionados ao controle de acesso baseado em função (RBAC).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar resourceOperations](../api/intune-rbac-resourceoperation-list.md)|Coleção [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Listar propriedades e relações dos objetos [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Obter resourceOperation](../api/intune-rbac-resourceoperation-get.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Ler propriedades e relações do objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Criar resourceOperation](../api/intune-rbac-resourceoperation-create.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Criar um novo objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Excluir resourceOperation](../api/intune-rbac-resourceoperation-delete.md)|Nenhum|Excluir um [resourceOperation](../resources/intune-rbac-resourceoperation.md)|
|[Atualizar resourceOperation](../api/intune-rbac-resourceoperation-update.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Atualizar as propriedades de um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[função getScopesForUser](../api/intune-rbac-resourceoperation-getscopesforuser.md)|String collection|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da operação de recurso. Somente leitura, gerada automaticamente.|
|recurso|String|Categoria de recurso à qual esta Operação pertence. Essa propriedade é somente leitura.|
|resourceName|Cadeia de caracteres|Nome do recurso em que essa operação é executada.|
|actionName|Cadeia de caracteres|Tipo de ação em que essa operação será executada. O actionName deve ser conciso e limitado ao mínimo de palavras possível.|
|description|String|Descrição da operação de recurso. A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.|
|enabledForScopeValidation|Boolean|Determina se a Permissão é validada para Escopos definidos por Atribuição de Função. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resource": "String",
  "resourceName": "String",
  "actionName": "String",
  "description": "String",
  "enabledForScopeValidation": true
}
```




