---
title: Criar ediscoveryCase
description: Crie um novo caso de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 319772b782a962d90c42b0ecf00baa728b8928fb
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945212"
---
# <a name="create-ediscoverycase"></a>Criar ediscoveryCase
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto ediscoveryCase](../resources/security-ediscoverycase.md) .

>[!NOTE]
> Essa API cria apenas um caso de Descoberta Eletrônica (Premium) usando o novo formato de caso. Para saber mais sobre o novo formato de caso na Descoberta Eletrônica, consulte Usar o novo formato de caso na [Descoberta Eletrônica (Premium)](/microsoft-365/compliance/advanced-ediscovery-new-case-format).
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto ediscoveryCase](../resources/security-ediscoverycase.md) .

Você pode especificar as propriedades a seguir ao criar **um ediscoveryCase**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome do caso de Descoberta Eletrônica. Obrigatório.|
|description|Cadeia de caracteres|A descrição do caso. Opcional.|
|externalId|Cadeia de caracteres|O número de caso externo para referência de cliente. Opcional.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` um código de resposta [e um objeto ediscoveryCase](../resources/security-ediscoverycase.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "create_ediscoverycase_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/ediscoveryCases
Content-Type: application/json

{
    "displayName": "CONTOSO LITIGATION-005",
    "description": "Project Bazooka",
    "externalId": "324516"
}
```


### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryCase"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases/$entity",
    "description": "Project Bazooka",
    "lastModifiedDateTime": "2022-05-22T18:36:48.0834353Z",
    "status": "active",
    "closedDateTime": "2022-05-22T18:36:48.083436Z",
    "externalId": "324516",
    "id": "22aa2acd-7554-4330-9ba9-ce20014aaae4",
    "displayName": "CONTOSO LITIGATION-005",
    "createdDateTime": "2022-05-22T18:36:48.0834351Z",
    "lastModifiedBy": null,
    "closedBy": null
}
```

