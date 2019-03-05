---
title: Tipo de recurso resourceOperation
description: Descreve o recurso ResourceOperation (entidade) da API do Microsoft Graph para o Intune (REST), que oferece suporte a cenários de controle de acesso baseado em função (RBAC) para organizações de locatários.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a299247815993a6ac1e99fe11ecead7ab66e2f2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164999"
---
# <a name="resourceoperation-resource-type"></a>Tipo de recurso resourceOperation

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Isso define uma operação ou ação que pode ser executada em um recurso (ou entidade) do Intune.  As operações comuns são Ler, Excluir, Atualizar ou Criar.  Essas operações fornecem gerenciamento básico do recurso do Intune subjacente em si.  Em alguns casos, um recurso do Intune pode ter operações usadas pelo recurso para agir em combinação com outros recursos.  Por exemplo, a operação Assign é usada para atribuir um recurso MobileApp a um grupo de segurança AAD.  Não é possível modificar as operações de recursos para funções internas. Isso define uma operação ou ação que pode ser executada em um recurso (ou entidade) do Intune.  As operações comuns são Obter, Listar, Excluir, Atualizar ou Criar.  Essas operações fornecem gerenciamento básico do recurso do Intune subjacente em si.  Em alguns casos, um recurso do Intune pode ter operações usadas pelo recurso para agir em combinação com outros recursos.  Por exemplo, a operação “Assign” é usada para atribuir um recurso MobileApp a um grupo de segurança AAD.  Não é possível modificar as operações de recursos para funções internas.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar resourceOperations](../api/intune-rbac-resourceoperation-list.md)|Coleção [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Listar propriedades e relações dos objetos [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Obter resourceOperation](../api/intune-rbac-resourceoperation-get.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Ler propriedades e relações do objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Criar resourceOperation](../api/intune-rbac-resourceoperation-create.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Criar um novo objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Excluir resourceOperation](../api/intune-rbac-resourceoperation-delete.md)|Nenhum|Excluir um [resourceOperation](../resources/intune-rbac-resourceoperation.md)|
|[Atualizar resourceOperation](../api/intune-rbac-resourceoperation-update.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Atualizar as propriedades de um objeto [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[função Getscopesforuser à](../api/intune-rbac-resourceoperation-getscopesforuser.md)|Coleção String|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da operação de recurso. Somente leitura, gerada automaticamente.|
|recurso|String|Categoria de recurso à qual essa operação pertence.|
|resourceName|Cadeia de caracteres|Nome do recurso em que essa operação é executada.|
|actionName|String|Tipo de ação em que essa operação será executada. O actionName deve ser conciso e limitado ao mínimo de palavras possível.|
|description|Cadeia de caracteres|Descrição da operação de recurso. A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.|
|enabledForScopeValidation|Boolean|Determina se a permissão é validada para os esCopos definidos por atribuição de função.|

## <a name="relationships"></a>Relações
Nenhuma

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




