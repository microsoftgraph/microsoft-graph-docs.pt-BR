---
title: Tipo de recurso extensionProperty
description: Representa uma extensão de diretório
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 23312e64c3812f5235a52380ef8acec65d206699
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123507"
---
# <a name="extensionproperty-resource-type"></a>Tipo de recurso extensionProperty

Namespace: microsoft.graph

Representa uma extensão de diretório que pode ser usada para adicionar uma propriedade personalizada a objetos de diretório sem exigir um armazenamento de dados externo. Por exemplo, se uma organização tiver um aplicativo LOB (linha de negócios) que exija uma ID de Skype para cada usuário no diretório, o Microsoft Graph poderá ser usado para registrar uma nova propriedade chamada skypeId no objeto User do diretório e, em seguida, gravar um valor na nova propriedade para um usuário específico.

Extensões podem ser adicionadas ao [usuário,](user.md) [grupo,](group.md) [organização,](organization.md) [dispositivo,](device.md) [recursos de](application.md) aplicativo. Somente 100 valores de extensão, em todos *os* tipos e todos os aplicativos, podem ser gravados em qualquer único recurso do Azure AD. 

> [!IMPORTANT]
> As extensões de esquema do Azure AD descritas aqui estão disponíveis no Microsoft Graph apenas por motivos de compatibilidade com compatibilidade.
> Ele permite que você use o Microsoft Graph para continuar a gerenciar propriedades de extensão adicionadas por meio do Azure AD Graph ou do [Azure AD Conexão](/azure/active-directory/hybrid/whatis-azure-ad-connect).
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
|isSyncedFromOnPremises|Boolean| Indica se essa propriedade de extensão foi sycned do diretório onpremises usando o Azure AD Conexão. Somente leitura. |
|name|Cadeia de caracteres| Nome da propriedade extension. Não anulável. |
|targetObjects|Coleção String| Os valores a seguir são suportados. Não anulável. <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

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
