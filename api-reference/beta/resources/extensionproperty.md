---
title: Tipo de recurso extensionProperty
description: Representa uma extensão de diretório
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8de2c18fb4f6ea5b6d2a91f453b915ee7f9b93ea
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556378"
---
# <a name="extensionproperty-resource-type"></a>Tipo de recurso extensionProperty

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma extensão de diretório que pode ser usada para adicionar uma propriedade personalizada a objetos de diretório sem exigir um armazenamento de dados externo. Por exemplo, se uma organização tiver um aplicativo de linha de negócios (LOB) que exija uma ID do Skype para cada usuário no diretório, o Microsoft Graph poderá ser usado para registrar uma nova propriedade chamada skypeId no objeto User do diretório e, em seguida, gravar um valor na nova propriedade para um usuário específico.

As extensões de diretório podem ser adicionadas aos seguintes objetos de diretório:
+ [user](user.md)
+ [group](group.md)
+ [organização](organization.md)
+ [device](device.md)
+ [recursos do](application.md) aplicativo

Somente 100 valores de extensão, *em todos os* tipos  e todos os aplicativos, podem ser gravados em qualquer instância de Azure AD recurso.

Use esse recurso e métodos associados para gerenciar as definições de extensão de diretório. Para gerenciar os dados de extensão de diretório na instância de recurso estendido, use a mesma solicitação REST que você usa para gerenciar a instância de recurso.

Para obter mais informações sobre a extensibilidade do Microsoft Graph, consulte [Adicionar propriedades personalizadas aos recursos usando extensões](/graph/extensibility-overview).

Herda de [directoryObject](directoryobject.md).

> [!NOTE]
> Extensões criadas por meio do Azure AD Graph (preterido) e dados personalizados sincronizados do Active Directory local usando o Azure AD Connect Sync são representadas como extensões de diretório no Microsoft Graph.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar extensionProperties](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | Criar uma propriedade de extensão em um objeto de aplicativo. |
| [Listar extensionProperties](../api/application-list-extensionproperty.md) | Coleção [extensionProperty](extensionProperty.md) | Listar propriedades de extensão em um objeto de aplicativo. |
| [Obter extensionProperty](../api/extensionproperty-get.md) | Coleção [extensionProperty](extensionProperty.md) | Listar propriedades de extensão em um objeto de aplicativo. |
| [Excluir extensionProperty](../api/extensionproperty-delete.md) | Nenhum | Excluir uma propriedade de extensão de um objeto de aplicativo. Você pode excluir somente as propriedades que não são sincronizadas do Active Directory local. |

> [!TIP]
> 1. Para definir um valor para a propriedade de extensão para uma instância de um recurso especificado em **targetObjects**, use a operação Atualizar do recurso. Por exemplo, a API [atualizar usuário](../api/user-update.md) para definir o valor de um usuário.
> 2. Para remover a propriedade de extensão e seu valor de uma instância de um recurso especificado em **targetObjects**, defina o valor da propriedade de extensão como `null`.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appDisplayName|Cadeia de caracteres| Nome de exibição do objeto de aplicativo no qual essa propriedade de extensão está definida. Somente leitura. |
|dataType|Cadeia de caracteres| Especifica o tipo de dados do valor que a propriedade de extensão pode conter. Há suporte para os valores a seguir. Não anulável. <ul><li>`Binary` - Máximo de 256 bytes</li><li>`Boolean`</li><li>`DateTime` - Deve ser especificado no formato ISO 8601. Serão armazenados no UTC.</li><li>`Integer` - Valor de 32 bits.</li><li>`LargeInteger` - Valor de 64 bits.</li><li>`String` - Máximo de 256 caracteres</li></ul>|
|deletedDateTime|DateTimeOffset|Data e hora em que este objeto foi excluído. Sempre `null` quando o objeto não tiver sido excluído. Herdado de [directoryObject](directoryobject.md).|
|isSyncedFromOnPremises|Booliano| Indica se essa propriedade de extensão foi sincronizada do Active Directory local usando o Azure AD Connect. Somente leitura. |
|name|String| Nome da propriedade de extensão. Não anulável. |
|targetObjects|Conjunto de cadeias de caracteres| Há suporte para os valores a seguir. Não anulável. <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.extensionProperty",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extensionProperty",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "name": "String",
  "dataType": "String",
  "isSyncedFromOnPremises": "Boolean",
  "targetObjects": [
    "String"
  ]
}
```

## <a name="see-also"></a>Confira também

+ [Adicionar propriedades personalizadas a recursos usando extensões](/graph/extensibility-overview)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
