---
title: Atualizar as ideias
description: Atualizar propriedades do objeto itemInsightsSettings
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: de19cf6f33ed0c5b1930077232945564115cd14a
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435002"
---
# <a name="update-iteminsightssettings"></a>Atualizar itemInsightsSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades do recurso [itemInsightsSettings](../resources/iteminsightssettings.md) especificado.

Para saber como personalizar a privacidade do item insights para sua organização, confira [Personalizar a privacidade do insights](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0). 

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | User.ReadWrite |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Application | User.ReadWrite |

>**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha uma função de administrador global.

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
|isEnabledInOrganization|Boolean| `true`Se o item de organização insights estiver habilitado; `false`se o item de organização insights estiver desabilitado para todos os usuários sem exceções. O padrão é `true`. Opcional.|
|disabledForGroup|Cadeia de caracteres| A ID de um grupo do Azure AD, do qual as insights do item dos membros estão desabilitadas. O padrão é `empty`. Opcional.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [itemInsightsSettings](../resources/iteminsightssettings.md) no corpo da resposta.

>**Observação:** Essa operação verifica a validade dos valores de Propriedade do recurso **itemInsightsSettings** especificado. Se a propriedade **disabledForGroup** estiver definida, essa operação não verifica a existência do grupo do Azure ad correspondente. Isso significa que, se você definir **disabledForGroup** como um grupo do Azure AD que não existe ou foi excluído posteriormente, essa operação não será capaz de identificar qualquer associação de grupo e desabilitar insights de item para qualquer usuário específico. Se **isEnabledInOrganization** estiver definido como `true` , a operação habilitará o insights para todos os usuários da organização. 

## <a name="example"></a>Exemplo 

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de solicitação de como o administrador atualiza a configuração de privacidade "**disabledForGroup**" para proibir a exibição de insights de item de usuários de um grupo específico do Azure AD.
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

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
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
