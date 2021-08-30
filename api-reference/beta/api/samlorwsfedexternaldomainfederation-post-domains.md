---
title: Criar externalDomainName
description: Crie um novo objeto externalDomainName.
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1eb7e580fb5e2c469eaece2889a236b4cde02b6d
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696995"
---
# <a name="create-externaldomainname"></a>Criar externalDomainName
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adicione vários domínios à sua configuração baseada em SAML ou WS-Fed criando um novo objeto [externalDomainName](../resources/externaldomainname.md) e adicione-o a um [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)existente.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|Domain.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|Domain.ReadWrite.All|

A conta de trabalho ou de estudante precisa pertencer a uma das seguintes [funções Azure Active Directory (Azure AD)](/azure/active-directory/roles/permissions-reference):

* Administrador global
* Administrador do Provedor de Identidade Externa

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /directory/federationConfigurations/{samlOrWsFedExternalDomainFederation ID}/microsoft.graph.samlOrWsFedExternalDomainFederation/domains
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto externalDomainName.](../resources/externaldomainname.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [externalDomainName](../resources/externaldomainname.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Nome de domínio da organização externa que você deseja adicionar ao [seu samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md). Herdado da [entidade](../resources/entity.md).|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto externalDomainName](../resources/externaldomainname.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_externaldomainname_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/directory/federationConfigurations/d5a56845-6845-d5a5-4568-a5d54568a5d5/microsoft.graph.samlOrWsFedExternalDomainFederation/domains
Content-Type: application/json
Content-length: 60

{
    "@odata.type": "microsoft.graph.externalDomainName",
    "id": "contososuites.com"
}
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalDomainName"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalDomainName",
  "id": "contososuites.com"
}
```
