---
title: Tipo de recurso applicationTemplate
description: Representa um aplicativo na galeria de aplicativos do Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c78834d027720371c1d259ce596fde82cb32ca46
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133207"
---
# <a name="applicationtemplate-resource-type"></a>Tipo de recurso applicationTemplate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um aplicativo na galeria [de aplicativos do Azure AD.](/azure/active-directory/saas-apps/tutorial-list)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[Lista applicationTemplate](../api/applicationtemplate-list.md)|[applicationTemplate](applicationtemplate.md)|Recupere uma lista de objetos applicationTemplate.|
| [Obter applicationTemplate](../api/applicationtemplate-get.md) | [applicationTemplate](applicationtemplate.md) | Leia as propriedades e os relacionamentos do objeto applicationTemplate. |
|[Instanciar o applicationtemplate](../api/applicationtemplate-instantiate.md)|[applicationServicePrincipal](applicationserviceprincipal.md)| Adicione uma instância de um aplicativo da galeria de aplicativos do Azure AD ao seu diretório.|


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|categories|Coleção de cadeias de caracteres|A lista de categorias do aplicativo. Os valores com suporte podem ser: `Collaboration` , , , , , , , , , , , `Business Management` , `Consumer` , `Content management` , `CRM` , , `Data services` , `Developer services` `E-commerce` `Education` `ERP` `Finance` `Health` `Human resources` e `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools, Travel` `Web design & hosting` .|
|description|String|Uma descrição do aplicativo.|
|displayName|String|O nome do aplicativo.|
|homePageUrl|String|A URL da página inicial do aplicativo.|
|id|String| Identificador exclusivo do aplicativo. Somente leitura.|
|logoUrl|String|A URL para obter o logotipo deste aplicativo.|
|publicador|String|O nome do editor deste aplicativo.|
|supportedProvisioningTypes|Coleção de cadeias de caracteres|A lista de modos de provisionamento suportados por esse aplicativo. O único valor válido é `sync` .|
|supportedSingleSignOnModes|Coleção de cadeias de caracteres|A lista de modos de login único suportados por esse aplicativo. Os valores com suporte são: `password`, `saml`, `external`, e `oidc`.|

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



