---
title: Tipo de recurso accessPackageResourceRequest
description: Uma solicitação de recurso do pacote de acesso é uma solicitação para adicionar um recurso a um catálogo para que as funções do recurso possam ser usadas em um ou mais pacotes de acesso do catálogo.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ea0d6ae14d93fbc691af4713cf40452a890d1891
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722185"
---
# <a name="accesspackageresourcerequest-resource-type"></a>Tipo de recurso accessPackageResourceRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma solicitação de recurso do pacote de acesso é uma solicitação para adicionar um recurso a um catálogo para que as funções do recurso possam ser usadas em um ou mais pacotes de acesso do catálogo ou para remover um recurso de um catálogo que não seja mais necessário pelos pacotes de acesso.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageResourceRequests](../api/accesspackageresourcerequest-list.md) | [Coleção accessPackageResourceRequest](accesspackageresourcerequest.md) | Recupere uma lista de **objetos accessPackageResourceRequest.** |
| [Criar accessPackageResourceRequest](../api/accesspackageresourcerequest-post.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | Crie um novo **objeto accessPackageResourceRequest.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|catalogId|Cadeia de caracteres|A ID exclusiva do catálogo de pacotes de acesso.|
|expirationDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|id|String| Somente leitura.|
|isValidationOnly|Booliano|Se definido, não adiciona o recurso.|
|justification|Cadeia de caracteres|A justificativa do solicitante para adicionar ou remover o recurso.|
|requestState|Cadeia de caracteres| O resultado se o serviço foi capaz de adicionar o recurso ao catálogo.  O valor é `Delivered` se o recurso foi adicionado ou removido. Somente Leitura.|
|requestStatus|String|Somente leitura.|
|requestType|Cadeia de caracteres|Use `AdminAdd` para adicionar um recurso, se o chamador for um administrador ou proprietário de recursos ou para remover um `AdminRemove` recurso. |

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageResource|[accessPackageResource](accesspackageresource.md)| Anulável.|
|requestor|[accessPackageSubject](accesspackagesubject.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "keyProperty": "id"
}-->

```json
{
  "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "expirationDateTime": "String (timestamp)",
  "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
  "isValidationOnly": false,
  "justification": "String",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "requestType": "AdminAdd"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


