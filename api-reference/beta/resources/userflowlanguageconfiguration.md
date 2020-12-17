---
title: tipo de recurso userFlowLanguageConfiguration
description: O objeto userFlowsLanguageConfiguration permite que um fluxo de usuário dê suporte à personalização de vários idiomas.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 69a32fbb3ec84928c9e4112134b6d771ca3149f4
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706225"
---
# <a name="userflowlanguageconfiguration-resource-type"></a>tipo de recurso userFlowLanguageConfiguration

Namespace: microsoft.graph

A personalização de idiomas de fluxos de usuário é um recurso que permite que um determinado fluxo de usuários dê suporte à personalização de vários idiomas, de todos os idiomas internos para um idioma personalizado.

Para os [fluxos de usuário do Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-language-customization#supported-languages), você pode aproveitar os idiomas internos ou fornecer as personalizações de idioma para um idioma que não esteja atualmente integrado por padrão. Para os [fluxos de usuário do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/external-identities/user-flow-customize-language), você só pode aproveitar os idiomas internos fornecidos pela Microsoft. Os dois fluxos de usuário do Azure Active Directory B2C e do Azure Active Directory dão suporte à personalização do idioma e às cadeias de caracteres mostradas aos usuários à medida que eles passam pelas viagens que você configura com seus fluxos de usuário.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-get.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Leia as propriedades e os relacionamentos de um objeto [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) . Esses objetos representam um idioma disponível em um fluxo de usuário.|
|[Excluir userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-delete.md)|Nenhum|Exclui um objeto [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) personalizado. Esses objetos representam um idioma disponível em um fluxo de usuário e apenas um idioma personalizado pode ser excluído de um fluxo de usuário do Azure AD B2C.|
|[Listar defaultpages](../api/userflowlanguageconfiguration-list-defaultpages.md)|coleção [userFlowLanguagePage](../resources/userflowlanguagepage.md)|Obtenha os recursos userFlowLanguagePage da propriedade de navegação defaultpages. Representa a jornada do usuário padrão em um fluxo de usuário.|
|[Listar overridesPages](../api/userflowlanguageconfiguration-list-overridespages.md)|coleção [userFlowLanguagePage](../resources/userflowlanguagepage.md)|Obtenha os recursos userFlowLanguagePage da propriedade de navegação overridesPages. Representa uma experiência personalizada para uma jornada do usuário em um fluxo de usuário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador do idioma. Este campo é a marca ID de idioma compatível com [RFC 5646](https://tools.ietf.org/html/rfc5646) e deve ser uma ID de idioma documentada.|
|isEnabled|Booliano|Indica se o idioma está habilitado dentro do fluxo do usuário.|
|displayName|Cadeia de caracteres|O nome do idioma a ser exibido. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|defaultpages|coleção [userFlowLanguagePage](../resources/userflowlanguagepage.md)|Conjunto de páginas com o conteúdo padrão a ser exibido em um fluxo de usuário para um idioma especificado. Essa coleção não permite qualquer tipo de modificação.|
|overridesPages|coleção [userFlowLanguagePage](../resources/userflowlanguagepage.md)|Conjunto de páginas com as mensagens de substituições a serem exibidas em um fluxo de usuário para um idioma especificado. Essa coleção permite apenas modificar o conteúdo da página, qualquer outra modificação não é permitida (criação ou exclusão de páginas).|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguageConfiguration",
  "id": "String (identifier)",
  "isEnabled": "Boolean",
  "displayName": "String"
}
```
