---
title: tipo de recurso accessPackageResource
description: Um recurso de pacote do Access é uma referência a um recurso associado a um catálogo as funções para as quais podem ser usadas em um ou mais pacotes de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8f862972b1c061d2c95267af19b26da300978288
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508524"
---
# <a name="accesspackageresource-resource-type"></a>tipo de recurso accessPackageResource

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure ad pretitulation Management](entitlementmanagement-root.md), um recurso de pacote do Access é uma referência a um recurso associado a um catálogo de pacotes do Access, as funções para as quais podem ser usadas em um ou mais pacotes de acesso.  Para solicitar a associação de um recurso a um catálogo de pacotes do Access, crie um [accessPackageResourceRequest](accesspackageresourcerequest.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar recursos do accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | coleção [accessPackageResource](accesspackageresource.md) | Recupere uma lista de objetos accessPackageResource em um catálogo. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|addedBy|String|Somente leitura.|
|adicionado|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|description|String|Uma descrição do recurso.|
|displayName|Cadeia de caracteres|O nome de exibição do recurso, como o nome do aplicativo, o nome do grupo ou o nome do site.|
|id|String| Somente leitura.|
|isPendingOnboarding|Boolean|True se o recurso ainda não está disponível para atribuição.|
|originid|String|O identificador exclusivo do recurso no sistema de origem. No caso de um grupo do Azure AD, esse é o identificador do grupo. |
|originSystem|String|O tipo do recurso no sistema de origem, como `SharePointOnline` ou. `AadGroup`|
|resourceType|String|O tipo do recurso, como `Application` se é um aplicativo conectado ao Azure ad ou `SharePoint Online Site` um site do SharePoint Online.|
|url|Cadeia de caracteres|Um localizador de recursos exclusivo para o recurso, como a URL para assinar um usuário em um aplicativo.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageResourceRoles|coleção [accessPackageResourceRole](accesspackageresourcerole.md)| Somente leitura. Anulável.|
|accessPackageResourceScopes|coleção [accessPackageResourceScope](accesspackageresourcescope.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResource",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "addedBy": "String",
  "addedOn": "String (timestamp)",
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
