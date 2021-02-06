---
title: Tipo de recurso accessPackageResource
description: Um recurso de pacote de acesso é uma referência a um recurso associado a um catálogo para as funções para as quais podem ser usadas em um ou mais pacotes de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 31499fda1d2d12f1e9868da6cf9e09fde38298cd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137463"
---
# <a name="accesspackageresource-resource-type"></a>Tipo de recurso accessPackageResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No Gerenciamento de Direitos do [Azure AD,](entitlementmanagement-root.md)um recurso de pacote de acesso é uma referência a um recurso associado a um catálogo de pacotes de acesso. As funções para o recurso do pacote de acesso podem ser usadas em um ou mais pacotes de acesso.  Para solicitar a associação de um recurso a um catálogo de pacotes de acesso ou remover um recurso de um catálogo, crie [um accessPackageResourceRequest](accesspackageresourcerequest.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar recursos accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | [Coleção accessPackageResource](accesspackageresource.md) | Recupere uma lista de objetos accessPackageResource em um catálogo. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageResourceEnvironment|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Contém as informações de ambiente do recurso. Isso pode ser definido usando a `@odata.bind` anotação ou o *originId do ambiente.*|
|addedBy|String|Somente leitura.|
|addedOn|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|description|String|Uma descrição para o recurso.|
|displayName|String|O nome de exibição do recurso, como o nome do aplicativo, o nome do grupo ou o nome do site.|
|id|String| Somente leitura.|
|isPendingOnboarding|Boolean|True se o recurso ainda não estiver disponível para atribuição.|
|originId|String|O identificador exclusivo do recurso no sistema de origem. No caso de um grupo do Azure AD, esse é o identificador do grupo. |
|originSystem|String|O tipo do recurso no sistema de origem, `SharePointOnline` como, `AadApplication` ou `AadGroup` .|
|resourceType|String|O tipo do recurso, como se fosse um aplicativo conectado ao Azure AD ou para um `Application` `SharePoint Online Site` site do SharePoint Online.|
|url|Cadeia de caracteres|Um localizador de recurso exclusivo para o recurso, como a URL para entrar um usuário em um aplicativo.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageResourceEnvironment|[accessPackageResourceEnvironment](accesspackageresourceenvironment.md)| Anulável.|
|accessPackageResourceRoles|[Coleção accessPackageResourceRole](accesspackageresourcerole.md)| Somente leitura. Anulável.|
|accessPackageResourceScopes|[Coleção accessPackageResourceScope](accesspackageresourcescope.md)| Somente leitura. Anulável.|

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
