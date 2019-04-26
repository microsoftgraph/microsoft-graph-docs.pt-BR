---
title: Atualizar governanceRoleSetting
description: Atualize as propriedades de governanceRoleSetting.
localization_priority: Normal
ms.openlocfilehash: d002317a4bf626f9a60cf98f6bd73b2075bf5727
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329666"
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
|Aplicativo | PrivilegedAccess. ReadWrite. AzureResources |

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
