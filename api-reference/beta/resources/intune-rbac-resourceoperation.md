---
title: Tipo de recurso resourceOperation
description: " operação é usada para atribuir um recurso de MobileApp a um grupo de segurança AAD.  Não é possível modificar as operações de recursos para funções internas."
ms.openlocfilehash: 2aed25c7558d674abb39fdb4147b722afe69c0f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034226"
---
# <a name="resourceoperation-resource-type"></a>Tipo de recurso resourceOperation

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Isso define uma operação ou ação que pode ser executada em um recurso (ou entidade) do Intune.  As operações comuns são Ler, Excluir, Atualizar ou Criar.  Essas operações fornecem gerenciamento básico do recurso do Intune subjacente em si.  Em alguns casos, um recurso do Intune pode ter operações usadas pelo recurso para agir em combinação com outros recursos.  Por exemplo, a operação Assign é usada para atribuir um recurso MobileApp a um grupo de segurança AAD.  Não é possível modificar as operações de recursos para funções internas. Isso define uma operação ou ação que pode ser executada em um recurso (ou entidade) do Intune.  As operações comuns são Obter, Listar, Excluir, Atualizar ou Criar.  Essas operações fornecem gerenciamento básico do recurso do Intune subjacente em si.  Em alguns casos, um recurso do Intune pode ter operações usadas pelo recurso para agir em combinação com outros recursos.  Por exemplo, a operação “Assign” é usada para atribuir um recurso MobileApp a um grupo de segurança AAD.  Não é possível modificar as operações de recursos para funções internas.
## <a name="methods"></a>Métodos
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
|id|Cadeia de caracteres|Chave da operação de recurso. Somente leitura, gerada automaticamente.|
|recurso|String|Categoria de recurso ao qual esta operação pertence.|
|resourceName|Cadeia de caracteres|Nome do recurso em que essa operação é executada.|
|actionName|Cadeia de caracteres|Tipo de ação em que essa operação será executada. O actionName deve ser conciso e limitado ao mínimo de palavras possível.|
|description|Cadeia de caracteres|Descrição da operação de recurso. A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.|
|enabledForScopeValidation|Booliano|Determina se a permissão é validada para escopos definidos por atribuição de função.|

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





