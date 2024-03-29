---
title: Tipo de recurso accessPackageCatalog
description: Um catálogo de pacotes de acesso é um contêiner para pacotes de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 556216ac7c7b51e18b2a918ccde63b5f730bf7d0
ms.sourcegitcommit: 0249c86925c9b4797908394c952073b5d9137911
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2022
ms.locfileid: "64477556"
---
# <a name="accesspackagecatalog-resource-type"></a>Tipo de recurso accessPackageCatalog

Namespace: microsoft.graph


No [gerenciamento de direitos do Azure AD](entitlementmanagement-overview.md), um catálogo de pacotes de acesso é um contêiner para zero ou mais pacotes de acesso. O gerenciamento de direitos do Azure AD inclui um catálogo integrado chamado **Geral**.

Um catálogo de pacotes de acesso também pode ter recursos vinculados usados nesses pacotes de acesso para fornecer acesso. Para exibir ou alterar a associação de funções com escopo de catálogo, use [a API de](unifiedroleassignment.md) atribuições de função com o provedor RBAC de gerenciamento de direitos.



## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessPackageCatalogs](../api/entitlementmanagement-list-catalogs.md)|[Coleção accessPackageCatalog](accesspackagecatalog.md)|Recupere uma lista de objetos accessPackageCatalog. |
|[Criar accessPackageCatalog](../api/entitlementmanagement-post-catalogs.md)|[accessPackageCatalog](accesspackagecatalog.md)|Crie um novo objeto accessPackageCatalog. |
|[Obter accessPackageCatalog](../api/accesspackagecatalog-get.md)|[accessPackageCatalog](accesspackagecatalog.md)|Ler propriedades e relações de um objeto accessPackageCatalog. |
|[Atualizar accessPackageCatalog](../api/accesspackagecatalog-update.md)|Nenhum|Atualize as propriedades de um objeto accessPackageCatalog. |
|[Excluir accessPackageCatalog](../api/accesspackagecatalog-delete.md)|Nenhum|Exclua accessPackageCatalog. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|catalogType|accessPackageCatalogType|Se o catálogo é criado por um usuário ou gerenciamento de direitos. Os valores possíveis são: `userManaged`, `serviceDefault`, `serviceManaged`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|description|Cadeia de caracteres|A descrição do catálogo de pacotes de acesso.|
|displayName|Cadeia de caracteres|O nome de exibição do catálogo de pacotes de acesso.|
|id|String|Somente leitura.|
|isExternallyVisible|Boolean|Se os pacotes de acesso neste catálogo podem ser solicitados por usuários fora do locatário.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |
|state|accessPackageCatalogState|Tem o valor `published` se os pacotes de acesso estão disponíveis para gerenciamento. Os valores possíveis são: `unpublished`, `published`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessPackages|[Coleção accessPackage](accesspackage.md)|Os pacotes de acesso neste catálogo. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageCatalog",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "catalogType": "String",
  "state": "String",
  "isExternallyVisible": "Boolean",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```


