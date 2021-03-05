---
title: Tipo de recurso applicationTemplate
description: Representa um aplicativo na galeria de aplicativos do Azure AD
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: dff7319444179dbe66698fa47691369ef3901340
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476410"
---
# <a name="applicationtemplate-resource-type"></a>Tipo de recurso applicationTemplate

Namespace: microsoft.graph

Representa um aplicativo na galeria de [aplicativos do Azure AD.](/azure/active-directory/saas-apps/tutorial-list)

## <a name="methods"></a>Métodos

| Método                                                                       | Tipo de retorno                                                   | Descrição                                                                                  |
| :--------------------------------------------------------------------------- | :------------------------------------------------------------ | :------------------------------------------------------------------------------------------- |
| [Lista applicationTemplate](../api/applicationtemplate-list.md)               | [applicationTemplate](applicationtemplate.md)                 | Recupere uma lista de objetos applicationTemplate.                                              |
| [Obter applicationTemplate](../api/applicationtemplate-get.md)                 | [applicationTemplate](applicationtemplate.md)                 | Ler propriedades e relações do objeto applicationTemplate.                             |
| [Instanciar o applicationtemplate](../api/applicationtemplate-instantiate.md) | [applicationServicePrincipal](applicationserviceprincipal.md) | Adicione uma instância de um aplicativo da galeria de aplicativos do Azure AD ao diretório. |

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo              | Descrição                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| :------------------------- | :---------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| categories                 | String collection | A lista de categorias do aplicativo. Os valores suportados podem ser: `Collaboration` , , , , , , , `Business Management` , , `Consumer` , , `Content management` , `CRM` `Data services` `Developer services` `E-commerce` `Education` `ERP` `Finance` `Health` `Human resources` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` , `Telecommunications` `Tools, Travel` `Web design & hosting` |
| description                | Cadeia de caracteres            | Uma descrição do aplicativo.                                                                                                                                                                                                                                                                                                                                                                                                               |
| displayName                | Cadeia de caracteres            | O nome do aplicativo.                                                                                                                                                                                                                                                                                                                                                                                                                    |
| homePageUrl                | Cadeia de caracteres            | A URL da home page do aplicativo.                                                                                                                                                                                                                                                                                                                                                                                                           |
| id                         | Cadeia de caracteres            | Identificador exclusivo do aplicativo. Somente leitura.                                                                                                                                                                                                                                                                                                                                                                                               |
| logoUrl                    | Cadeia de caracteres            | A URL para obter o logotipo desse aplicativo.                                                                                                                                                                                                                                                                                                                                                                                                   |
| publicador                  | String            | O nome do editor deste aplicativo.                                                                                                                                                                                                                                                                                                                                                                                                 |
| supportedProvisioningTypes | Conjunto de cadeias de caracteres | A lista de modos de provisionamento suportados por esse aplicativo. O único valor válido é `sync` .                                                                                                                                                                                                                                                                                                                                                   |
| supportedSingleSignOnModes | Conjunto de cadeias de caracteres | A lista de modos de login único suportados por este aplicativo. Os valores com suporte são: `oidc`, `password`, `saml`, e `notSupported`.                                                                                                                                                                                                                                                                                                            |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "keyProperty": "id"
}-->

```json
{
  "id": "id-value",
  "displayName": "displayName-value",
  "homePageUrl": "homePageUrl-value",
  "supportedSingleSignOnModes": ["supportedSingleSignOnModes-value"],
  "logoUrl": "logoUrl-value",
  "categories": ["categories-value"],
  "publisher": "publisher-value",
  "description": "description-value"
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
