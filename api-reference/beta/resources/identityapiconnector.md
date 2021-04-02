---
title: Tipo de recurso identityApiConnector
description: Representa conectores de API em um locatário do Azure Active Directory.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7ecb96a9ca2f4397c1f0ee52908a7802374df0f
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508074"
---
# <a name="identityapiconnector-resource-type"></a>Tipo de recurso identityApiConnector

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa conectores de API em um Azure Active Directory (Azure AD) e locatários do Azure AD B2C.

Um conector de API usado na sua assinatura de autoatendados de Identidades Externas do Azure AD e fluxos de usuário de entrada do Azure AD B2C permite que você chame uma API durante a execução do fluxo de usuários. Um conector de API fornece as informações necessárias para chamar uma API, incluindo uma URL de ponto de extremidade e autenticação. Um conector de API pode ser usado em uma etapa específica em um fluxo de usuário para afetar a execução do fluxo do usuário. Por exemplo, a resposta da API pode impedir que um usuário se inscreve, mostrar um erro de validação de entrada ou substituir atributos coletados pelo usuário.

Use a [API b2xIdentityUserFlow](b2xidentityuserflow.md) para usar um conector de API de um fluxo de usuário de autoatendência de Identidades Externas.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List](../api/identityapiconnector-list.md)|[Coleção identityApiConnector](identityapiconnector.md)| Obter uma lista de conectores de API|
|[Criar](../api/identityapiconnector-create.md)|[identityApiConnector](identityapiconnector.md)|Crie um novo conector de API. |
|[Obter](../api/identityapiconnector-get.md)|[identityApiConnector](identityapiconnector.md)|Leia as propriedades de [um objeto identityApiConnector.](../resources/identityapiconnector.md)|
|[Atualizar](../api/identityapiconnector-update.md)|[identityApiConnector](identityapiconnector.md)|Atualize as propriedades de um conector de API.|
|[Carregar certificado do cliente](../api/identityapiconnector-uploadclientcertificate.md)|[identityApiConnector](identityapiconnector.md)|Carregar um certificado de cliente a ser usado para autenticação.|
|[Delete](../api/identityapiconnector-delete.md)|Nenhum|Exclua um conector de API.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID gerada aleatoriamente do conector da API. |
|displayName|Cadeia de caracteres| O nome do conector da API. |
|targetUrl|Cadeia de caracteres| A URL do ponto de extremidade da API a ser chamada. |
|authenticationConfiguration|[apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)|O objeto que descreve os detalhes de configuração de autenticação para chamar a API. Certificado cliente básico e PKCS 12 são suportados.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityApiConnector",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityApiConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "targetUrl": "String",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
  }
}
```
