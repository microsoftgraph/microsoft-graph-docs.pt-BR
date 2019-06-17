---
title: Tipo de recurso resourceOperation
description: Descreve o recurso resourceOperation (entidade) da API do Microsoft Graph (REST), que oferece suporte a fluxos de trabalho do Intune relacionados ao controle de acesso baseado em função (RBAC).
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2ac5cdcfbf444a0cc8642da16ca93aac9ccca65
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993575"
---
# <a name="resourceoperation-resource-type"></a>Tipo de recurso resourceOperation

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve o recurso resourceOperation (entidade) da API do Microsoft Graph (REST), que oferece suporte a fluxos de trabalho do Intune relacionados ao controle de acesso baseado em função (RBAC).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar resourceOperations](../api/intune-rbac-resourceoperation-list.md)|Coleção [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Listar propriedades e relações dos objetos [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Obter resourceOperation](../api/intune-rbac-resourceoperation-get.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Ler propriedades e relações do objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Criar resourceOperation](../api/intune-rbac-resourceoperation-create.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Criar um novo objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Excluir resourceOperation](../api/intune-rbac-resourceoperation-delete.md)|Nenhum|Excluir um [resourceOperation](../resources/intune-rbac-resourceoperation.md)|
|[Atualizar resourceOperation](../api/intune-rbac-resourceoperation-update.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Atualizar as propriedades de um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[função Getscopesforuser à](../api/intune-rbac-resourceoperation-getscopesforuser.md)|String collection|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da operação de recurso. Somente leitura, gerada automaticamente.|
|recurso|String|Categoria de recurso à qual essa operação pertence.|
|resourceName|Cadeia de caracteres|Nome do recurso em que essa operação é executada.|
|actionName|Cadeia de caracteres|Tipo de ação em que essa operação será executada. O actionName deve ser conciso e limitado ao mínimo de palavras possível.|
|descrição|String|Descrição da operação de recurso. A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.|
|enabledForScopeValidation|Booliano|Determina se a permissão é validada para os escopos definidos por atribuição de função.|

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





