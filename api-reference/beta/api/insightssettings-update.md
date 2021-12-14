---
title: Atualizar insights
description: Atualizar propriedades do objeto insightsSettings
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: d4ff6298e6266d24a8b490bcbefc4ea30eea1d3c
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339490"
---
# <a name="update-insightssettings"></a>Atualizar insightsSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as configurações de privacidade para exibir ou retornar o tipo especificado de insights em uma organização. O tipo de configuração pode ser insights de item ou informações de pessoas.

Para saber mais sobre como personalizar a privacidade de insights para sua organização, consulte:
-  [Personalizar privacidade de insights de item](/graph/insights-customize-item-insights-privacy) 
-  [Personalizar privacidade de insights de pessoas](/graph/insights-customize-people-insights-privacy)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é necessária para chamar essa API. Para saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |


>**Observação:** O uso de permissões delegadas para essa operação exige que o usuário inscreveu tenha uma função de administrador global.
## <a name="http-request"></a>Solicitação HTTP

Para atualizar as configurações para insights de item:
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/itemInsights
```

Para atualizar configurações para informações de pessoas:
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/peopleInsights
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
|isEnabledInOrganization|Boolean| `true` se o tipo especificado de insights estiver habilitado para a organização; `false` se o tipo especificado de insights estiver desabilitado para todos os usuários sem exceções. O padrão é `true`. Opcional.|
|disabledForGroup|String| A ID de um grupo do Azure AD, do qual o tipo especificado de insights está desabilitado para seus membros. O padrão é `empty`. Opcional.|

>**Observação:** Esta operação não verifica o valor **da propriedade disabledForGroup** se você o incluir no corpo da solicitação. Se você definir a **propriedade disabledForGroup** como uma cadeia de caracteres, essa operação não verificará a existência do grupo correspondente do Azure AD. Isso significa que, se você definir **disabledForGroup** para um grupo do Azure AD que não existe ou é excluído posteriormente, essa operação não será capaz de identificar qualquer associação de grupo e desabilitar informações de itens ou pessoas para usuários específicos. Se **isEnabledInOrganization** estiver definido como , a operação habilita o tipo especificado de insights para todos os `true` usuários da organização.  
## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto insightsSettings](../resources/insightssettings.md) no corpo da resposta.

## <a name="examples"></a>Exemplos 

### <a name="example-1-update-settings-for-item-insights"></a>Exemplo 1: Atualizar configurações para insights de item
#### <a name="request"></a>Solicitação

Aqui está um exemplo de solicitação que mostra como um administrador atualiza a configuração de privacidade "**disabledForGroup**" para proibir a exibição de insights de item de usuários em um grupo específico do Azure AD.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_insightssettings_iteminsightrequest"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
Content-type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-insightssettings-iteminsightrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-insightssettings-iteminsightrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-insightssettings-iteminsightrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-insightssettings-iteminsightrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-insightssettings-iteminsightrequest-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.insightsSettings",
  "name": "update_insightssettings_iteminsightrequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


### <a name="example-2-update-settings-for-people-insights"></a>Exemplo 2: Atualizar configurações para informações de pessoas
#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação que mostra como um administrador atualiza a configuração de privacidade "**disabledForGroup**" para proibir a exibição de informações de pessoas de usuários em um grupo específico do Azure AD.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_insightssettings_peopleinsightsrequest"
}-->
```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/peopleInsights
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-insightssettings-peopleinsightsrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-insightssettings-peopleinsightsrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-insightssettings-peopleinsightsrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-insightssettings-peopleinsightsrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-insightssettings-peopleinsightsrequest-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a>Resposta

Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.insightsSettings",
  "name": "update_insightssettings_peopleinsightsrequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


 107 api-reference/beta/api/iteminsightssettings-get.md 
