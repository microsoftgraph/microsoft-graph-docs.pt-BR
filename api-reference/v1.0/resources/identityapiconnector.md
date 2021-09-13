---
title: Tipo de recurso identityApiConnector
description: Representa conectores de API em um Azure Active Directory locatário.
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 05c51b2468885daea730e597b2c4f7172699c28f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098962"
---
# <a name="identityapiconnector-resource-type"></a>Tipo de recurso identityApiConnector

Namespace: microsoft.graph

Representa conectores de API em Azure Active Directory locatários do Azure AD.

Um conector de API usado em seus fluxos de usuário de autoatendados de identidades externas do Azure AD permite que você chame uma API durante a execução do fluxo do usuário. Um conector de API fornece as informações necessárias para chamar uma API, incluindo uma URL de ponto de extremidade e autenticação. Um conector de API pode ser usado em uma etapa específica em um fluxo de usuário para afetar a execução do fluxo do usuário. Por exemplo, a resposta da API pode impedir que um usuário se inscreve, mostrar um erro de validação de entrada ou substituir atributos coletados pelo usuário.

Use a [API b2xIdentityUserFlow](b2xidentityuserflow.md) para usar um conector de API de um fluxo de usuário de autoatendência de Identidades Externas.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List](../api/identityapiconnector-list.md)|Coleção [identityApiConnector](../resources/identityapiconnector.md)| Obter uma lista de conectores de API|
|[Criar](../api/identityapiconnector-create.md)|[identityApiConnector](identityapiconnector.md)|Crie um novo conector de API. |
|[Obter](../api/identityapiconnector-get.md)|[identityApiConnector](identityapiconnector.md)|Leia as propriedades de [um objeto identityApiConnector.](../resources/identityapiconnector.md)|
|[Atualizar](../api/identityapiconnector-update.md)|[identityApiConnector](identityapiconnector.md)|Atualize as propriedades de um conector de API.|
|[Upload cliente](../api/identityapiconnector-uploadclientcertificate.md)|[identityApiConnector](identityapiconnector.md)|Upload um certificado de cliente a ser usado para autenticação.|
|[Delete](../api/identityapiconnector-delete.md)|None|Exclua um conector de API.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador gerado aleatoriamente do conector de API. |
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
