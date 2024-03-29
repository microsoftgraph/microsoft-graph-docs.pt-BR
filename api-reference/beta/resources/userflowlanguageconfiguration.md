---
title: Tipo de recurso userFlowLanguageConfiguration
description: O objeto userFlowsLanguageConfiguration permite que um fluxo de usuários suporte à personalização de vários idiomas.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: aa83d85725cbef54229cdc92246fb83888697166
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547145"
---
# <a name="userflowlanguageconfiguration-resource-type"></a>Tipo de recurso userFlowLanguageConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A personalização do idioma de fluxo do usuário é um recurso que permite que um determinado fluxo de usuários suporte à personalização de vários idiomas, de todos os idiomas integrados a um idioma personalizado.

Para Azure Active Directory fluxos de usuários [B2C,](/azure/active-directory-b2c/user-flow-language-customization#supported-languages)você pode aproveitar os idiomas integrados ou fornecer as personalizações de idioma para um idioma que não está integrado no momento por padrão. Para [Azure Active Directory fluxos de usuário](/azure/active-directory/external-identities/user-flow-customize-language), você só pode aproveitar os idiomas integrados fornecidos pela Microsoft. Os fluxos de usuários para Azure Active Directory B2C e Azure Active Directory suportam personalizar o idioma e as cadeias de caracteres mostradas aos usuários à medida que passam pelas jornadas que você configura com seus fluxos de usuário.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-get.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Leia as propriedades e as relações de um [objeto userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md) Esses objetos representam um idioma disponível em um fluxo de usuários.|
|[Excluir userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-delete.md)|Nenhum|Exclui um objeto [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) personalizado. Esses objetos representam um idioma disponível em um fluxo de usuário e somente um idioma personalizado pode ser excluído de um fluxo de usuário do Azure AD B2C.|
|[Listar defaultPages](../api/userflowlanguageconfiguration-list-defaultpages.md)|[Coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)|Obter os recursos userFlowLanguagePage da propriedade de navegação defaultPages. Representa a jornada padrão do usuário em um fluxo de usuários.|
|[Lista substituiPages](../api/userflowlanguageconfiguration-list-overridespages.md)|[Coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)|Obter os recursos userFlowLanguagePage da propriedade de navegação overridesPages. Representa uma experiência personalizada para uma jornada do usuário em um fluxo de usuários.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do idioma. Este campo é a marca de identificação de idioma [RFC 5646](https://tools.ietf.org/html/rfc5646) compatível e deve ser uma ID de idioma documentada.|
|isEnabled|Booliano|Indica se o idioma está habilitado no fluxo do usuário.|
|displayName|String|O nome do idioma a ser exibido. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|defaultPages|[Coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)|Coleção de páginas com o conteúdo padrão a ser exibido em um fluxo de usuário para um idioma especificado. Essa coleção não permite nenhum tipo de modificação.|
|overridesPages|[Coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)|O conjunto de páginas com as mensagens substitui a exibição em um fluxo de usuário para um idioma especificado. Essa coleção só permite modificar o conteúdo da página, qualquer outra modificação não é permitida (criação ou exclusão de páginas).|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration",
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
