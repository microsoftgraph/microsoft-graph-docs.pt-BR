---
title: Atualizar groupLifecyclePolicy
description: Atualiza as propriedades de um objeto do tipo de recurso groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f2e7e7fd27566476e224d5c58cbd12803b6c38aa
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262717"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="3d08e-103">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="3d08e-103">Update groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d08e-104">Atualiza as propriedades de um objeto do [tipo de recurso groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3d08e-104">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d08e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d08e-105">Permissions</span></span>

<span data-ttu-id="3d08e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d08e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="3d08e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d08e-108">Permission type</span></span>      | <span data-ttu-id="3d08e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d08e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d08e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d08e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d08e-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d08e-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="3d08e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d08e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d08e-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3d08e-113">Not supported</span></span> |
|<span data-ttu-id="3d08e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d08e-114">Application</span></span> | <span data-ttu-id="3d08e-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d08e-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d08e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d08e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3d08e-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="3d08e-117">Optional request headers</span></span>
| <span data-ttu-id="3d08e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3d08e-118">Name</span></span> | <span data-ttu-id="3d08e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d08e-119">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="3d08e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d08e-120">Authorization</span></span> | <span data-ttu-id="3d08e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d08e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d08e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3d08e-123">Content-Type</span></span>  | <span data-ttu-id="3d08e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3d08e-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3d08e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d08e-125">Request body</span></span>

<span data-ttu-id="3d08e-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3d08e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3d08e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d08e-129">Property</span></span> | <span data-ttu-id="3d08e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d08e-130">Type</span></span> | <span data-ttu-id="3d08e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d08e-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3d08e-132">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="3d08e-132">alternateNotificationEmails</span></span>|<span data-ttu-id="3d08e-133">String</span><span class="sxs-lookup"><span data-stu-id="3d08e-133">String</span></span>| <span data-ttu-id="3d08e-134">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="3d08e-134">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="3d08e-135">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="3d08e-135">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="3d08e-136">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="3d08e-136">groupLifetimeInDays</span></span>|<span data-ttu-id="3d08e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3d08e-137">Int32</span></span>| <span data-ttu-id="3d08e-138">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="3d08e-138">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="3d08e-139">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="3d08e-139">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="3d08e-140">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="3d08e-140">managedGroupTypes</span></span>|<span data-ttu-id="3d08e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d08e-141">String</span></span>| <span data-ttu-id="3d08e-142">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="3d08e-142">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="3d08e-143">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="3d08e-143">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="3d08e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d08e-144">Response</span></span>

<span data-ttu-id="3d08e-145">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d08e-145">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3d08e-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d08e-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3d08e-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d08e-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 151

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="3d08e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d08e-148">Response</span></span>
<span data-ttu-id="3d08e-149">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="3d08e-149">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3d08e-150">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3d08e-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3d08e-151">C#</span><span class="sxs-lookup"><span data-stu-id="3d08e-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_grouplifecyclepolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d08e-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="3d08e-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_grouplifecyclepolicy-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3d08e-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3d08e-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_grouplifecyclepolicy-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
