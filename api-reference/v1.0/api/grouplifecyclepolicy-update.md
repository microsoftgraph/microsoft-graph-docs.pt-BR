---
title: Atualizar groupLifecyclePolicy
description: Atualiza as propriedades de um objeto do tipo de recurso groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9cdbe988e38f6af1941df9eeb2565538295cea28
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273252"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="f7038-103">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f7038-103">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="f7038-104">Atualiza as propriedades de um objeto do [tipo de recurso groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f7038-104">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7038-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7038-105">Permissions</span></span>

<span data-ttu-id="f7038-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 
|<span data-ttu-id="f7038-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7038-108">Permission type</span></span>      | <span data-ttu-id="f7038-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7038-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7038-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7038-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7038-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7038-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7038-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7038-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7038-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7038-113">Not supported.</span></span>    |
|<span data-ttu-id="f7038-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7038-114">Application</span></span> | <span data-ttu-id="f7038-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7038-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7038-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7038-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="f7038-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="f7038-117">Optional request headers</span></span>
| <span data-ttu-id="f7038-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f7038-118">Name</span></span> | <span data-ttu-id="f7038-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7038-119">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="f7038-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7038-120">Authorization</span></span> | <span data-ttu-id="f7038-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7038-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7038-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7038-123">Content-Type</span></span>  | <span data-ttu-id="f7038-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f7038-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7038-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7038-125">Request body</span></span>

<span data-ttu-id="f7038-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f7038-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f7038-127">As propriedades existentes que não estão incluídas no corpo da solicitação mantêm os valores anteriores ou recalcula-os com base nas alterações feitas em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f7038-127">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="f7038-128">Para obter o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f7038-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f7038-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7038-129">Property</span></span> | <span data-ttu-id="f7038-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7038-130">Type</span></span> | <span data-ttu-id="f7038-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7038-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f7038-132">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="f7038-132">alternateNotificationEmails</span></span>|<span data-ttu-id="f7038-133">String</span><span class="sxs-lookup"><span data-stu-id="f7038-133">String</span></span>| <span data-ttu-id="f7038-134">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="f7038-134">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="f7038-135">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="f7038-135">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="f7038-136">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="f7038-136">groupLifetimeInDays</span></span>|<span data-ttu-id="f7038-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f7038-137">Int32</span></span>| <span data-ttu-id="f7038-138">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="f7038-138">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="f7038-139">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="f7038-139">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="f7038-140">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="f7038-140">managedGroupTypes</span></span>|<span data-ttu-id="f7038-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7038-141">String</span></span>| <span data-ttu-id="f7038-142">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="f7038-142">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="f7038-143">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="f7038-143">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="f7038-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7038-144">Response</span></span>

<span data-ttu-id="f7038-145">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7038-145">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7038-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7038-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f7038-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7038-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="f7038-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7038-148">Response</span></span>
<span data-ttu-id="f7038-149">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f7038-149">Note: The response object shown here may be truncated for brevity.</span></span> 
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f7038-150">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f7038-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f7038-151">C#</span><span class="sxs-lookup"><span data-stu-id="f7038-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_grouplifecyclepolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7038-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="f7038-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_grouplifecyclepolicy-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f7038-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f7038-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_grouplifecyclepolicy-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
