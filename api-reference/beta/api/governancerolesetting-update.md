---
title: Atualizar governanceRoleSetting
description: Atualize as propriedades de governanceRoleSetting.
localization_priority: Normal
ms.openlocfilehash: 73a6d8ea95d4f691cef9fc3610f7e997e9fb5be8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263515"
---
# <a name="update-governancerolesetting"></a>Atualizar governanceRoleSetting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [governanceRoleSetting](../resources/governancerolesetting.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

>**Observação:** Essa API também exige que o solicitante tenha pelo menos uma `Active` atribuição de função de`owner` administrador `user access administrator`(ou) no recurso.

|Tipo de permissão      | Permissões              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | PrivilegedAccess. ReadWrite. AzureResources  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:-----------|:-----------|
| Authorization  | Portador {código}|
| Content-type  | application/json|


## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para [governanceRuleSettings](../resources/governancerulesetting.md) que precisam ser atualizados. 

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|adminEligibleSettings|coleção [governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função qualificada.|
|adminMemberSettings|coleção [governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.|
|userEligibleSettings|coleção [governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra que são avaliadas quando um usuário tenta adicionar uma atribuição de função qualificada. Isso não é suportado para `pimforazurerbac` o cenário por enquanto, e pode estar disponível nos cenários futuros.|
|userMemberSettings|coleção [governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra que são avaliadas quando um usuário tenta ativar sua atribuição de função.|

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta. 

### <a name="error-codes"></a>Códigos de erro
Essa API retorna os códigos de erro HTTP padrão. Além disso, ele retorna os seguintes códigos de erro personalizados.

|Código de erro     | Mensagem de erro         | Detalhes             |
|:--------------| :---------------------|:--------------------|
| 400 BadRequest| RoleSettingNotFound   | O [governanceRoleSetting](../resources/governancerolesetting.md) não existe no sistema.
| 400 BadRequest| InvalidRoleSetting    | Os valores de [governanceRuleSettings](../resources/governancerulesetting.md) fornecidos no corpo da solicitação não são válidos.

## <a name="example"></a>Exemplo 
Este exemplo atualiza a configuração de função para a função 3 personalizada na assinatura Wingtip Toys-prod.
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
   "adminEligibleSettings":[
      {
         "ruleIdentifier":"ExpirationRule",
         "setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
      }
   ]
}
```
##### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/update_governancerolesetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_governancerolesetting-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_governancerolesetting-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
