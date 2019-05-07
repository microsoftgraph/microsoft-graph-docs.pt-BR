---
title: Atualizar secureScoreControlProfile
description: Atualize um objeto secureScoreControlProfile editável em qualquer solução integrada para alterar várias propriedades, como assignedTo ou tenantNote.
author: preetikr
localization_priority: Normal
ms.openlocfilehash: 8f3193b72ac59528c386bb6207b17d4440e6c98a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629744"
---
# <a name="update-securescorecontrolprofile"></a>Atualizar secureScoreControlProfile

Atualize um objeto **secureScoreControlProfile** editável em qualquer solução integrada para alterar várias propriedades, como **assignedTo** ou **tenantNote**.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |   Escopo securityevents. ReadWrite. All.  |
|Delegado (conta pessoal da Microsoft) |  Sem suporte.  |
|Application | Escopo securityevents. ReadWrite. All. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização  | Portador {código}. Obrigatório.|
|Preferir | Return = representação. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON dos valores de campos relevantes que devem ser atualizados. O corpo **deve** conter a `vendorInformation` Propriedade com os `provider` campos `vendor` válidos e. A tabela a seguir lista os campos que podem ser atualizados para um **secureScoreControlProfile**. Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|assignedTo|Cadeia de caracteres|Nome do analista ao qual o controle é atribuído para a triagem, implementação ou correção.|
|comment|String|Comentários de analista sobre o controle (para o gerenciamento de controle de clientes).|
|state| Cadeia de caracteres|Configuração orientada pelo analista no controle. Os valores possíveis são: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.|
| vendorInformation | [securityVendorInformation](../resources/securityvendorinformation.md) | Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = SecureScore;). **Os campos Provider e Vendor são necessários.** |


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

Se o cabeçalho de solicitação opcional for usado, o método retornará `200 OK` um código de resposta e o objeto [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="example-1-request-without-prefer-header"></a>Exemplo 1: solicitação sem cabeçalho de preferência

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/NonOwnerAccess
Content-type: application/json

{
  "assignedTo": "",
  "comment": "control is reviewed",
  "state": "Reviewed",
  "vendorInformation": {

    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

### <a name="response"></a>Resposta

Veja a seguir o exemplo de uma resposta bem-sucedida.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>Exemplo 2: solicitação com cabeçalho preferencial

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação que inclui `Prefer` o cabeçalho da solicitação.

<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/NonOwnerAccess
Content-type: application/json

{
  "assignedTo": "",
  "comment": "control is reviewed",
  "state": "Reviewed",
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta quando o cabeçalho de `Prefer: return=representation` solicitação opcional é usado.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "NonOwnerAccess",
  "azureTenantId": "00000001-0001-0001-0001-000000000001c",
  "actionType": "Review",
  "actionUrl": "https://outlook.office365.com/NonOwnerAccessReport.aspx",
  "controlCategory": "Data",
  "title": "Review mailbox access by non-owners bi-weekly", 
  "deprecated": false,
  "implementationCost": "Low",
  "lastModifiedDateTime": null,
  "maxScore": 5.0,
  "rank": 25,
  "remediation": "Once you have opened the search tool, specify a date range and select access by <b>All non-owners</b> or <b>External users</b>",
  "remediationImpact": "This change will have no effect on your users",
  "service": "EXO",
  "threats": [
    "Account Breach",
    "Data Exfiltration",
    "Malicious Insider"
  ],
  "tier": "Core",
  "userImpact": "Low",
  "complianceInformation": [
    {
      "certificationName": "FedRAMP_Moderate",
      "certificationControls": [
        {
          "name": "AC-6(9)",
          "url": "",
        }
      ]
    }         
  ],
  "controlStateUpdates": [
    {
      "assignedTo": "",
      "comment": "control is reviewed",
      "state": "Reviewed",
      "updatedBy": "user1@contoso.com",
      "updatedDateTime": "2019-03-19T22:37:14.628799Z"
    }
  ],
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
