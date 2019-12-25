---
title: tipo de recurso applicationtemplate
description: Representa um aplicativo na Galeria de aplicativos do Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0c34c083a4cfee63db724228d9390c7452ca5a92
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870943"
---
# <a name="applicationtemplate-resource-type"></a>tipo de recurso applicationtemplate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um aplicativo na [Galeria de aplicativos do Azure ad](/azure/active-directory/saas-apps/tutorial-list).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[Listar aplicativo](../api/applicationtemplate-list.md)|[applicationtemplate](applicationtemplate.md)|Recupere uma lista de objetos applicationtemplate.|
| [Obter applicationtemplate](../api/applicationtemplate-get.md) | [applicationtemplate](applicationtemplate.md) | Leia as propriedades e as relações do objeto applicationtemplate. |
|[Instanciar applicationtemplate](../api/applicationtemplate-instantiate.md)|[applicationServicePrincipal](applicationserviceprincipal.md)| Adicione uma instância de um aplicativo da Galeria de aplicativos do Azure AD ao seu diretório.|


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|categories|Coleção de cadeias de caracteres|A lista de categorias para o aplicativo. Os valores com suporte podem `Collaboration`ser `Business Management`: `Consumer`,`Content management`, `CRM`, `Data services` `Developer services` `E-commerce` `Education` `ERP` `Finance` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools, Travel`,,,,,,,,,,,,,,,,,,,,,,,,,, e `Web design & hosting` `Health` `Human resources`|
|descrição|String|Uma descrição do aplicativo.|
|displayName|Cadeia de caracteres|O nome do aplicativo.|
|homePageUrl|String|A URL da home page do aplicativo.|
|id|String| Identificador exclusivo do aplicativo. Somente leitura.|
|logoUrl|String|A URL para obter o logotipo para este aplicativo.|
|publicador|String|O nome do editor para este aplicativo.|
|supportedProvisioningTypes|Coleção de cadeias de caracteres|A lista de modos de provisionamento compatíveis com este aplicativo. O único valor válido é `sync`.|
|supportedSingleSignOnModes|Coleção de cadeias de caracteres|A lista de modos de logon único suportados por este aplicativo. Os valores com suporte `password`são `saml`, `external`, e `oidc`.|

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
