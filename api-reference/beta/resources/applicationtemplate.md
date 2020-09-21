---
title: tipo de recurso applicationtemplate
description: Representa um aplicativo na Galeria de aplicativos do Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1dcb5d1a4f1a86521081487ec66494d76c035b82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050231"
---
# <a name="applicationtemplate-resource-type"></a>tipo de recurso applicationtemplate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um aplicativo na [Galeria de aplicativos do Azure ad](/azure/active-directory/saas-apps/tutorial-list).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[Lista applicationTemplate](../api/applicationtemplate-list.md)|[applicationTemplate](applicationtemplate.md)|Recupere uma lista de objetos applicationtemplate.|
| [Obter applicationtemplate](../api/applicationtemplate-get.md) | [applicationTemplate](applicationtemplate.md) | Leia as propriedades e as relações do objeto applicationtemplate. |
|[Instanciar o applicationtemplate](../api/applicationtemplate-instantiate.md)|[applicationServicePrincipal](applicationserviceprincipal.md)| Adicione uma instância de um aplicativo da Galeria de aplicativos do Azure AD ao seu diretório.|


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Categorias|Coleção de cadeias de caracteres|A lista de categorias para o aplicativo. Os valores com suporte podem ser:,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `Collaboration` `Business Management` `Consumer` `Content management` `CRM` `Data services` `Developer services` `E-commerce` `Education` `ERP` `Finance` `Health` `Human resources` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools, Travel` e `Web design & hosting` .|
|description|String|Uma descrição do aplicativo.|
|displayName|Cadeia de caracteres|O nome do aplicativo.|
|homePageUrl|Cadeia de caracteres|A URL da home page do aplicativo.|
|id|Cadeia de caracteres| Identificador exclusivo do aplicativo. Somente leitura.|
|logoUrl|Cadeia de caracteres|A URL para obter o logotipo para este aplicativo.|
|publicador|String|O nome do editor para este aplicativo.|
|supportedProvisioningTypes|Coleção de cadeias de caracteres|A lista de modos de provisionamento compatíveis com este aplicativo. O único valor válido é `sync` .|
|supportedSingleSignOnModes|Coleção de cadeias de caracteres|A lista de modos de logon único suportados por este aplicativo. Os valores com suporte são `password` , `saml` , `external` e `oidc` .|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


