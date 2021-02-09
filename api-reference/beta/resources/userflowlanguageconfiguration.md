---
title: Tipo de recurso userFlowLanguageConfiguration
description: O objeto userFlowsLanguageConfiguration permite que um fluxo de usuário suporte a personalização de vários idiomas.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c9c963fcb7f22af34de92d0ad1c9a472974e346f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159791"
---
# <a name="userflowlanguageconfiguration-resource-type"></a>Tipo de recurso userFlowLanguageConfiguration

Namespace: microsoft.graph

O usuário flui a personalização de idioma é um recurso que permite que um determinado fluxo de usuário suporte a personalização de vários idiomas, de todos os idiomas integrados para um idioma personalizado.

Para fluxos de usuário do [Azure Active Directory B2C,](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-language-customization#supported-languages)você pode aproveitar os idiomas integrados ou fornecer as personalizações de idioma para um idioma que não está atualmente integrado por padrão. Para fluxos de usuário do [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/external-identities/user-flow-customize-language)você só pode aproveitar os idiomas integrados fornecidos pela Microsoft. Ambos os fluxos de usuário para o Azure Active Directory B2C e o Azure Active Directory suportam personalizar o idioma e as cadeias de caracteres mostradas aos usuários durante as jornadas que você configura com seus fluxos de usuário.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-get.md)|[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)|Leia as propriedades e os relacionamentos de um [objeto userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md) Esses objetos representam um idioma disponível em um fluxo de usuário.|
|[Excluir userFlowLanguageConfiguration](../api/userflowlanguageconfiguration-delete.md)|Nenhum(a)|Exclui um objeto [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) personalizado. Esses objetos representam um idioma disponível em um fluxo de usuário e apenas um idioma personalizado pode ser excluído de um fluxo de usuário do Azure AD B2C.|
|[Listar defaultPages](../api/userflowlanguageconfiguration-list-defaultpages.md)|[Coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)|Obter os recursos userFlowLanguagePage da propriedade de navegação defaultPages. Representa a jornada do usuário padrão em um fluxo de usuário.|
|[Listar overridesPages](../api/userflowlanguageconfiguration-list-overridespages.md)|[Coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)|Obter os recursos userFlowLanguagePage da propriedade de navegação overridesPages. Representa uma experiência personalizada para uma jornada do usuário em um fluxo de usuário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do idioma. Esse campo é compatível com a marca de identificação de idioma [RFC 5646](https://tools.ietf.org/html/rfc5646) e deve ser uma ID de idioma documentada.|
|isEnabled|Booliano|Indica se o idioma está habilitado dentro do fluxo do usuário.|
|displayName|String|O nome do idioma a ser exibido. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|defaultPages|[Coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)|Coleção de páginas com o conteúdo padrão a ser exibido em um fluxo de usuário para um idioma especificado. Essa coleção não permite qualquer tipo de modificação.|
|overridesPages|[Coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)|Coleção de páginas com as mensagens de substituição a exibir em um fluxo de usuário para um idioma especificado. Essa coleção só permite modificar o conteúdo da página, qualquer outra modificação não é permitida (criação ou exclusão de páginas).|

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
