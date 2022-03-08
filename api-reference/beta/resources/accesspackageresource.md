---
title: Tipo de recurso accessPackageResource
description: Um recurso de pacote de acesso é uma referência a um recurso associado a um catálogo para o qual as funções podem ser usadas em um ou mais pacotes de acesso.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 06ecfec829481fde26ceb6dbe810f6c567dc66ea
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336064"
---
# <a name="accesspackageresource-resource-type"></a>Tipo de recurso accessPackageResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](entitlementmanagement-overview.md), um recurso de pacote de acesso é uma referência a um recurso associado a um catálogo de pacotes de acesso. As funções do recurso de pacote de acesso podem ser usadas em um ou mais pacotes de acesso.  Para solicitar a associação de um recurso a um catálogo de pacotes de acesso ou remover um recurso de um catálogo, crie [um accessPackageResourceRequest](accesspackageresourcerequest.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar recursos do accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | [Coleção accessPackageResource](accesspackageresource.md) | Recupere uma lista de objetos accessPackageResource em um catálogo. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|attributes|[coleção accessPackageResourceAttribute](../resources/accesspackageresourceattribute.md)| Contém informações sobre os atributos a serem coletados do solicitante e enviados para o aplicativo de recurso. |
|addedBy|String|O nome do usuário ou aplicativo que adicionou esse recurso pela primeira vez. Somente leitura.|
|addedOn|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|description|Cadeia de caracteres|Uma descrição do recurso.|
|displayName|String|O nome de exibição do recurso, como nome do aplicativo, nome do grupo ou nome do site.|
|id|String| Somente leitura.|
|isPendingOnboarding|Booliano|True se o recurso ainda não estiver disponível para atribuição.|
|originId|Cadeia de caracteres|O identificador exclusivo do recurso no sistema de origem. No caso de um grupo do Azure AD, esse é o identificador do grupo. |
|originSystem|String|O tipo do recurso no sistema de origem, como `SharePointOnline`, `AadApplication` ou `AadGroup`.|
|resourceType|Cadeia de caracteres|O tipo do recurso, como `Application` se for um aplicativo conectado ao Azure AD ou `SharePoint Online Site` para um site SharePoint Online.|
|url|Cadeia de caracteres|Um localizador de recurso exclusivo para o recurso, como a URL para assinar um usuário em um aplicativo.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageResourceEnvironment|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Contém as informações de ambiente do recurso. Isso pode ser definido usando `@odata.bind` a anotação ou a *originId do ambiente*. Dá suporte a `$expand`.|
|accessPackageResourceRoles|[Coleção accessPackageResourceRole](accesspackageresourcerole.md)| Somente leitura. Anulável. Suporta o `$expand`.|
|accessPackageResourceScopes|[Coleção accessPackageResourceScope](accesspackageresourcescope.md)| Somente leitura. Anulável. Suporta o `$expand`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResource",
  "keyProperty": "id"
}-->

```json
{
  "addedBy": "String",
  "addedOn": "String (timestamp)",
  "attributes": [
    {
      "@odata.type": "microsoft.graph.accessPackageResourceAttribute"
    }
   ],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isPendingOnboarding": true,
  "originId": "String",
  "originSystem": "String",
  "resourceType": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
