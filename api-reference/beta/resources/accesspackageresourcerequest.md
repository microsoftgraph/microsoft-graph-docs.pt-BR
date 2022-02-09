---
title: Tipo de recurso accessPackageResourceRequest
description: Uma solicitação de recurso do pacote de acesso é uma solicitação para adicionar um recurso a um catálogo para que as funções do recurso possam ser usadas em um ou mais pacotes de acesso do catálogo.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9f6557a4256b692005c82ca18bc93041f003b886
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468287"
---
# <a name="accesspackageresourcerequest-resource-type"></a>Tipo de recurso accessPackageResourceRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD](entitlementmanagement-overview.md), uma solicitação de recurso do pacote de acesso é uma solicitação para adicionar um recurso a um catálogo para que as funções do recurso possam ser usadas em um ou mais pacotes de acesso do catálogo ou para remover um recurso de um catálogo que não seja mais necessário pelos pacotes de acesso.[](accesspackageresource.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageResourceRequests](../api/entitlementmanagement-list-accesspackageresourcerequests.md) | [Coleção accessPackageResourceRequest](accesspackageresourcerequest.md) | Recupere uma lista de **objetos accessPackageResourceRequest** . |
| [Criar accessPackageResourceRequest](../api/entitlementmanagement-post-accesspackageresourcerequests.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | Crie um novo **objeto accessPackageResourceRequest** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|catalogId|String|A ID exclusiva do catálogo de pacotes de acesso.|
|expirationDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|id|String| Somente leitura.|
|isValidationOnly|Boolean|Se definido, não adiciona o recurso.|
|justification|String|A justificativa do solicitante para adicionar ou remover o recurso.|
|requestState|Cadeia de caracteres| O resultado se o serviço foi capaz de adicionar o recurso ao catálogo.  O valor é `Delivered` se o recurso foi adicionado ou removido. Somente Leitura.|
|requestStatus|String|Somente leitura.|
|requestType|Cadeia de caracteres|Use `AdminAdd` para adicionar um recurso, se o chamador for um administrador ou proprietário de recursos ou `AdminRemove` para remover um recurso. |

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageResource|[accessPackageResource](accesspackageresource.md)| Anulável.|
|requestor|[accessPackageSubject](accesspackagesubject.md)| Somente leitura. Anulável. Suporta o `$expand`.|

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


