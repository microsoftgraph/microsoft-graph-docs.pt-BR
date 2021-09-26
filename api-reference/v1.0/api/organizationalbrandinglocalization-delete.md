---
title: Excluir organizationalBrandingLocalization
description: Exclui um objeto organizationalBrandingLocalization.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 62df5020c5fb29a2e8987fbc25ec11fd1a5684ee
ms.sourcegitcommit: 7ce66321abb6a2cdca8685d3ce0a004c376ae33b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777985"
---
# <a name="delete-organizationalbrandinglocalization"></a>Excluir organizationalBrandingLocalization
Namespace: microsoft.graph

Exclua um objeto de identidade visual localizado. Para excluir o [objeto organizationalBrandingLocalization,](../resources/organizationalbrandinglocalization.md) todas as imagens (tipos de fluxo) devem primeiro ser removidas do objeto.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Organization.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /organization/{organizationId}/branding/localizations/{organizationalBrandingLocalizationId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

A seguir, um exemplo de uma solicitação para excluir o `fr-FR` objeto de localização.

<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandinglocalization"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR
```


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

