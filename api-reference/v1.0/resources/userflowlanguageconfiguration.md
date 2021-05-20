---
title: tipo de recurso userFlowLanguageConfiguration
description: Permite que um fluxo de usuário suporte vários idiomas.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 556860eb77c4707f1d180b7924ae3126958a4799
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547201"
---
# <a name="userflowlanguageconfiguration-resource-type"></a>tipo de recurso userFlowLanguageConfiguration

Namespace: microsoft.graph

Permite que um fluxo de usuário suporte o uso de vários idiomas.

Para [Azure Active Directory fluxos de usuários,](/azure/active-directory/external-identities/user-flow-customize-language)você só pode aproveitar os idiomas incorporados fornecidos pela Microsoft. O usuário flui para Azure Active Directory suporte definindo o idioma e as strings mostradas aos usuários à medida que passam pelas jornadas que você configura com os fluxos do usuário.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obtenha configuração do userFlowLanguage](../api/userflowlanguageconfiguration-get.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Leia as propriedades e relacionamentos de um objeto de [Configuração do usuárioFlowLanguage.](../resources/userflowlanguageconfiguration.md) Esses objetos representam uma linguagem disponível em um fluxo de usuário.|
|[Liste páginas padrão](../api/userflowlanguageconfiguration-list-defaultpages.md)|[coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)|Obtenha os recursos do userFlowLanguagePage da propriedade de navegação padrãoPages. Representa a jornada padrão do usuário em um fluxo de usuário.|
|[Lista substitui Páginas](../api/userflowlanguageconfiguration-list-overridespages.md)|[coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)|Obtenha os recursos do userFlowLanguagePage da propriedade de navegação overridesPages. Representa uma experiência personalizada para uma jornada do usuário em um fluxo de usuário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador da linguagem. Este campo é compatível com a tag [RFC 5646](https://tools.ietf.org/html/rfc5646) e deve ser um ID de idioma documentado.|
|isEnabled|Booliano|Indica se o idioma está ativado dentro do fluxo do usuário.|
|displayName|Cadeia de caracteres|O nome do idioma para exibir. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|páginas padrão|[coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)|Coleção de páginas com o conteúdo padrão para exibir em um fluxo de usuário para um idioma especificado. Esta coleção não permite qualquer tipo de modificação.|
|substitui Páginas|[coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)|A coleção de páginas com as mensagens substituidas para exibir em um fluxo de usuário para um idioma especificado. Esta coleção só permite modificar o conteúdo da página, qualquer outra modificação não é permitida (criação ou exclusão de páginas).|

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
