---
title: Atualizar itemInsights
description: Atualizar propriedades do objeto itemInsightsSettings
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 43ee5650c87d2cbf21a0a8b1c35a05e7874b9cab
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020785"
---
# <a name="update-iteminsightssettings"></a>Atualizar itemInsightsSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar propriedades do recurso [itemInsightsSettings](../resources/iteminsightssettings.md) especificado.

Para saber como personalizar a privacidade de insights de item para sua organização, consulte [personalizar a privacidade de insights.](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0) 

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

>**Observação:** O uso de permissões delegadas para essa operação exige que o usuário inscreveu tenha uma função de administrador global.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor|
|:-----------|:------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Booliano| `true` se as percepções do item da organização estão habilitadas; `false` se as percepções do item da organização estão desabilitadas para todos os usuários sem exceções. O padrão é `true`. Opcional.|
|disabledForGroup|Cadeia de caracteres| A ID de um grupo do Azure AD, do qual as informações do item dos membros estão desabilitadas. O padrão é `empty`. Opcional.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [itemInsightsSettings](../resources/iteminsightssettings.md) no corpo da resposta.

>**Observação:** Esta operação verifica a validade dos valores de propriedade do **recurso itemInsightsSettings** especificado. Se a **propriedade disabledForGroup** estiver definida, essa operação não verificará a existência do Grupo do Azure AD correspondente. Isso significa que, se você definir **disabledForGroup** para um grupo do Azure AD que não existia ou foi excluído posteriormente, essa operação não poderá identificar nenhuma associação de grupo e desabilitar informações de item para usuários específicos. Se **isEnabledInOrganization** estiver definido como , a operação permitirá insights `true` para todos os usuários na organização. 

## <a name="example"></a>Exemplo 

### <a name="request"></a>Solicitação

Aqui está um exemplo de solicitação sobre como o administrador atualiza a configuração de privacidade "**disabledForGroup**" para proibir a exibição de informações de item dos usuários de um grupo específico do Azure AD.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_iteminsightssettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
Content-type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-iteminsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-iteminsightssettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta

Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemInsightsSettings",
  "name": "update_iteminsightssettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


