---
title: Tipo de recurso extensionProperty
description: Representa uma extensão de diretório
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 93b5c066895bcc3b8adc801bd7f8bf8283cc3535
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961983"
---
# <a name="extensionproperty-resource-type"></a>Tipo de recurso extensionProperty

Namespace: microsoft.graph

Representa uma extensão de diretório que pode ser usada para adicionar uma propriedade personalizada a objetos de diretório sem exigir um armazenamento de dados externo. Por exemplo, se uma organização tiver um aplicativo LOB (linha de negócios) que exija uma ID do Skype para cada usuário no diretório, o Microsoft Graph poderá ser usado para registrar uma nova propriedade chamada skypeId no objeto User do diretório e, em seguida, gravar um valor na nova propriedade para um usuário específico.

Extensões podem ser adicionadas ao [usuário,](user.md) [grupo,](group.md) [organização,](organization.md) [dispositivo,](device.md) [recursos de](application.md) aplicativo. Somente 100 valores de extensão, em todos *os* tipos e todos os aplicativos, podem ser gravados em qualquer único recurso do Azure AD. 

> [!IMPORTANT]
> As extensões de esquema do Azure AD descritas aqui estão disponíveis no Microsoft Graph apenas por motivos de compatibilidade com compatibilidade com vertidas.
> Ele permite que você use o Microsoft Graph para continuar a gerenciar propriedades de extensão adicionadas por meio do Azure AD Graph ou [do Azure AD Connect](/azure/active-directory/hybrid/whatis-azure-ad-connect).
> Para novas extensões personalizadas, recomendamos que você use extensões de esquema do Microsoft Graph para adicionar [dados personalizados aos recursos](/graph/extensibility-overview).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar extensão](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | Criar uma propriedade de extensão em um objeto de aplicativo. |
| [Listar extensões](../api/application-list-extensionproperty.md) | Coleção [extensionProperty](extensionProperty.md) | Listar propriedades de extensão em um objeto de aplicativo. |
| [Excluir extensão](../api/application-delete-extensionproperty.md) | Nenhum | Excluir uma propriedade de extensão de um objeto de aplicativo. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appDisplayName|Cadeia de caracteres| Nome de exibição do objeto application no qual essa propriedade de extensão é definida. Somente leitura. |
|dataType|Cadeia de caracteres| Especifica o tipo de dados do valor que a propriedade extension pode manter. Os valores a seguir são suportados. Não anulável. <ul><li>`Binary` - Máximo de 256 bytes</li><li>`Boolean`</li><li>`DateTime` - Deve ser especificado no formato ISO 8601. Serão armazenados no UTC.</li><li>`Integer` - Valor de 32 bits.</li><li>`LargeInteger` - Valor de 64 bits.</li><li>`String` - Máximo de 256 caracteres</li></ul>|
|isSyncedFromOnPremises|Booliano| Indica se essa propriedade de extensão foi sycned do diretório onpremises usando o Azure AD Connect. Somente leitura. |
|name|Cadeia de caracteres| Nome da propriedade extension. Não anulável. |
|targetObjects|Coleção de cadeias de caracteres| Os valores a seguir são suportados. Não anulável. <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionProperty",
  "keyProperty": "id"
}-->

```json
{
  "appDisplayName": "String",
  "dataType": "String",
  "isSyncedFromOnPremises": true,
  "name": "String",
  "targetObjects": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
