---
title: Tipo de recurso identityApiConnector
description: Representa conectores de API em um locatário do Azure Active Directory.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e5b3c10e6a03c4868e010f8f62f0f073ce37ca61
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161646"
---
# <a name="identityapiconnector-resource-type"></a>Tipo de recurso identityApiConnector

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa conectores de API em um Azure Active Directory (Azure AD) e locatários do Azure AD B2C.

Um conector de API usado em sua assinatura de identidades externas do Azure AD e fluxos de usuário de assinatura do Azure AD B2C permite que você chame uma API durante a execução do fluxo do usuário. Um conector de API fornece as informações necessárias para chamar uma API, incluindo uma URL de ponto de extremidade e autenticação. Um conector de API pode ser usado em uma etapa específica em um fluxo de usuário para afetar a execução do fluxo do usuário. Por exemplo, a resposta da API pode impedir que um usuário se inscreve, mostrar um erro de validação de entrada ou substituir atributos coletados pelo usuário.

Use a API [b2xIdentityUserFlow](b2xidentityuserflow.md) para usar um conector de API de um fluxo de usuário de entrada de autoatendente identidades externas.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List](../api/identityapiconnector-list.md)|[Coleção identityApiConnector](identityapiconnector.md)| Obter uma lista de conectores de API|
|[Criar](../api/identityapiconnector-create.md)|[identityApiConnector](identityapiconnector.md)|Crie um novo conector de API. |
|[Get](../api/identityapiconnector-get.md)|[identityApiConnector](identityapiconnector.md)|Leia as propriedades de um [objeto identityApiConnector.](../resources/identityapiconnector.md)|
|[Update](../api/identityapiconnector-update.md)|[identityApiConnector](identityapiconnector.md)|Atualizar as propriedades de um conector de API.|
|[Delete](../api/identityapiconnector-delete.md)|Nenhum(a)|Exclua um conector de API.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID gerada aleatoriamente do conector da API. |
|displayName|String| O nome do conector da API. |
|targetUrl|String| A URL do ponto de extremidade da API a ser chamada. |
|authenticationConfiguration|[apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)|O objeto que descreve os detalhes de configuração de autenticação para chamar a API. Somente [a autenticação](basicauthentication.md) Básica é suportada no momento.|

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
