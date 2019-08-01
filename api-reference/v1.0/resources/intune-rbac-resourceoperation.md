---
title: Tipo de recurso resourceOperation
description: Descreve o recurso resourceOperation (entidade) da API do Microsoft Graph (REST), que oferece suporte a fluxos de trabalho do Intune relacionados ao controle de acesso baseado em função (RBAC).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f3519255524c38d75b941461682f2538a6ee39a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037132"
---
# <a name="resourceoperation-resource-type"></a>Tipo de recurso resourceOperation

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

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da operação de recurso. Somente leitura, gerada automaticamente.|
|resourceName|Cadeia de caracteres|Nome do recurso em que essa operação é executada.|
|actionName|Cadeia de caracteres|Tipo de ação em que essa operação será executada. O actionName deve ser conciso e limitado ao mínimo de palavras possível.|
|descrição|String|Descrição da operação de recurso. A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.|

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
  "resourceName": "String",
  "actionName": "String",
  "description": "String"
}
```



