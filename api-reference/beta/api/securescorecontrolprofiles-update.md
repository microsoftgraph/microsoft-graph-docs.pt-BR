---
title: Atualizar secureScoreControlProfiles
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: b89a5e147d4882dbe25456cd2acc42b56924d12b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817651"
---
# <a name="update-securescorecontrolprofiles"></a>Atualizar secureScoreControlProfiles

 > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Atualize uma propriedade editável **secureScoreControlProfiles** dentro de qualquer solução integrada para alterar várias propriedades, como **assignedTo** ou **tenantNote**.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |   SecurityEvents.ReadWrite.All.  |
|Delegado (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | SecurityEvents.ReadWrite.All. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização  | Portador {código}. Obrigatório.|
|Preferir | retornar = representação. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON dos valores para os campos relevantes que devem ser atualizados. A tabela a seguir lista os campos que podem ser atualizados por um secureScoreControlProfile. Os valores para propriedades existentes que não estão incluídos no corpo da solicitação não serão alterado. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|assignedTo|Cadeia de caracteres|Nome do analista de controle é atribuída a triagem, implementação ou correção.|
|tenantNote|Cadeia de caracteres|Comentários de analistas no controle (para gerenciamento de controle do cliente).|
|controlStateUpdates| Cadeia de caracteres|Analista orientada a configuração no controle. Os valores possíveis são: `ignore`, `thirdParty`, `reviewed`.|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

Se o cabeçalho de solicitação opcional for usado, o método retornará um `200 OK` código de resposta e o objeto atualizado [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "assignedTo": "assignedTo-value",
  "controlStateUpdates": "controlStateUpdates-value",
  "tenantNote": "tenantNote-value"
}
```

### <a name="response"></a>Resposta

O exemplo a seguir é um exemplo de uma resposta bem-sucedida.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```




<!-- {
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
