---
title: tipo de recurso identityApiConnector
description: Representa conectores de API em um locatário do Azure Active Directory.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6098b146b5117332df36b76adcbce95698d6041d
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720096"
---
# <a name="identityapiconnector-resource-type"></a>tipo de recurso identityApiConnector

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os conectores de API em um Azure Active Directory (Azure AD) e locatários do Azure AD B2C.

Um conector de API usado em suas identidades externas do Azure AD inscrição de autoatendimento e os fluxos de usuário de inscrição do Azure AD B2C permitem chamar uma API durante a execução do fluxo do usuário. Um conector de API fornece as informações necessárias para chamar uma API, incluindo uma URL de ponto de extremidade e autenticação. Um conector de API pode ser usado em uma etapa específica em um fluxo de usuário para afetar a execução do fluxo do usuário. Por exemplo, a resposta da API pode impedir que um usuário se inscrever, mostrar um erro de validação de entrada ou substituir os atributos coletados pelo usuário.

Use a API [b2xIdentityUserFlow](b2xidentityuserflow.md) para usar um conector de API de um fluxo de usuário de inscrição de autoatendimento de identidade externa.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List](../api/identityapiconnector-list.md)|coleção [identityApiConnector](identityapiconnector.md)| Obter uma lista de conectores de API|
|[Create](../api/identityapiconnector-create.md)|[identityApiConnector](identityapiconnector.md)|Criar um novo conector de API. |
|[Get](../api/identityapiconnector-get.md)|[identityApiConnector](identityapiconnector.md)|Ler as propriedades de um objeto [identityApiConnector](../resources/identityapiconnector.md) .|
|[Update](../api/identityapiconnector-update.md)|[identityApiConnector](identityapiconnector.md)|Atualizar as propriedades de um conector de API.|
|[Delete](../api/identityapiconnector-delete.md)|Nenhum|Excluir um conector de API.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID gerada aleatoriamente do conector da API. |
|displayName|Cadeia de caracteres| O nome do conector da API. |
|targetUrl|Cadeia de caracteres| A URL do ponto de extremidade da API a ser chamado. |
|authenticationConfiguration|[apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)|O objeto que descreve os detalhes de configuração de autenticação para chamar a API. Só há suporte para a [autenticação básica](basicauthentication.md) no momento.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityApiConnector",
  "baseType": "",
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
