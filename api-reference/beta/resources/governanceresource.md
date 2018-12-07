---
title: tipo de recurso de governanceResource
description: Representa os recursos que pôde ser gerenciados pelo gerenciamento de identidade privilegiado (PIM). Para obter recursos Azure, pode ser uma assinatura, um grupo de recursos e um recurso como uma máquina virtual, um banco de dados do SQL, etc.
ms.openlocfilehash: 6a048680c3b9bb614287e764d547a20bd09b5d25
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191127"
---
# <a name="governanceresource-resource-type"></a>tipo de recurso de governanceResource

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa os recursos que pôde ser gerenciados pelo gerenciamento de identidade privilegiado (PIM). Para obter recursos Azure, pode ser uma assinatura, um grupo de recursos e um recurso como uma máquina virtual, um banco de dados do SQL, etc.


## <a name="methods"></a>Métodos

| Método          | Tipo de retorno |Descrição|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | coleção [governanceResource](../resources/governanceresource.md)|Uma coleção de recursos para que o solicitante tem acesso de lista.|
|[Get](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |As propriedades de leitura e relacionamentos de uma entidade de recurso especificado pelo id.|
|[Registro](../api/governanceresource-register.md) | |Registre um não gerenciado grupo Azure de assinatura ou de gerenciamento ao serviço PIM. |

Não `POST`, `PUT`, `PATCH`, `DELETE` são suportados no `roleDefinitions` conjunto de entidade para agora.

## <a name="properties"></a>Propriedades
| Propriedade          |Tipo         |Descrição|
|:------------------|:----------|:----------|
|id                 |String     |A identificação do recurso. Ela está no formato GUID.|
|externalId           |Cadeia de caracteres   |A id externa do recurso, que representa seu id original no sistema externo. Por exemplo, id externo de um recurso assinatura pode ser "/ assinaturas/c14ae696-5e0c-4e5d-88cc-bef6637737ac". |
|type               |String     |Obrigatório. Tipo de recurso. Por exemplo, para recursos do Windows Azure, o tipo poderia ser "Assinatura", "ResourceGroup", "Microsoft.Sql/server", etc.|
|displayName        |String     |O nome de exibição do recurso.|
|status             |String     |O status de um determinado recurso. Por exemplo, poderia representar se o recurso está bloqueado ou não (valores: `Active` / `Locked`). Observação: Essa propriedade pode ser estendida no futuro para oferecer suporte a mais cenários.|
|registeredDateTime|DateTimeOffset      |Representa a data hora quando o recurso é registrado no PIM.|
|registeredRoot|String      |ExternalId do escopo de raiz do recurso que está registrado no PIM. O escopo de raiz pode ser o pai, avô ou recursos de ancestral superior.|
|roleAssignmentCount|Int32      |Opcional. O número de atribuições de função para o recurso determinado. Para obter a propriedade, faça uso explicitamente `$select=roleAssignmentCount` na consulta.|
|roleDefinitionCount|Int32      |Opcional. O número de definições de função para o recurso determinado. Para obter a propriedade, faça uso explicitamente `$select=roleDefinitionCount` na consulta.|
|permissions|[governancePermission](../resources/governancepermission.md)      |Opcional. Representa o status de acesso do solicitador para o recurso. Para obter a propriedade, faça uso explicitamente `$select=permissions` na consulta.|

## <a name="relationships"></a>Relações
| Relação   | Tipo                                         |Descrição|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)|A coleção de atribuições de função para o recurso.|
|roleDefinitions |coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)|A coleção de definições de função para o recurso.|
|roleAssignmentRequests |coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|A coleção de solicitações de atribuição de função para o recurso.|
|roleSettings |coleção [governanceRoleSetting](../resources/governancerolesetting.md)|A coleção de configurações de função para o recurso.|
|pai          |[governanceResource](../resources/governanceresource.md)           |Somente leitura. O recurso de pai. para `pimforazurerbac` cenário, ela pode representar a assinatura que o recurso pertence.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceResource"
}-->
```json
{
  "id": "String (identifier)",
  "externalId": "String",
  "type": "String",
  "displayName": "String",
  "status": "String",
  "registeredDateTime": "String (timestamp)",
  "registeredRoot": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
