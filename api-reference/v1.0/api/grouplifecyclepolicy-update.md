---
title: Atualizar groupLifecyclePolicy
description: Atualiza as propriedades de um objeto do tipo de recurso groupLifecyclePolicy.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e5c422287c241f2ce9d9d1507114e8795df0dd5e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053059"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="18a1c-103">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="18a1c-103">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="18a1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18a1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18a1c-105">Atualiza as propriedades de um objeto do [tipo de recurso groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="18a1c-105">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="18a1c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="18a1c-106">Permissions</span></span>

<span data-ttu-id="18a1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18a1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 
|<span data-ttu-id="18a1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18a1c-109">Permission type</span></span>      | <span data-ttu-id="18a1c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18a1c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18a1c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18a1c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="18a1c-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a1c-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="18a1c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18a1c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18a1c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18a1c-114">Not supported.</span></span>    |
|<span data-ttu-id="18a1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18a1c-115">Application</span></span> | <span data-ttu-id="18a1c-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a1c-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18a1c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18a1c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="18a1c-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="18a1c-118">Optional request headers</span></span>
| <span data-ttu-id="18a1c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="18a1c-119">Name</span></span> | <span data-ttu-id="18a1c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a1c-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="18a1c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="18a1c-121">Authorization</span></span> | <span data-ttu-id="18a1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18a1c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18a1c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18a1c-124">Content-Type</span></span>  | <span data-ttu-id="18a1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18a1c-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18a1c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18a1c-126">Request body</span></span>

<span data-ttu-id="18a1c-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="18a1c-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="18a1c-128">As propriedades existentes que não estão incluídas no corpo da solicitação mantêm os valores anteriores ou recalcula-os com base nas alterações feitas em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="18a1c-128">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="18a1c-129">Para obter o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="18a1c-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="18a1c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18a1c-130">Property</span></span> | <span data-ttu-id="18a1c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="18a1c-131">Type</span></span> | <span data-ttu-id="18a1c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a1c-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="18a1c-133">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="18a1c-133">alternateNotificationEmails</span></span>|<span data-ttu-id="18a1c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a1c-134">String</span></span>| <span data-ttu-id="18a1c-135">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="18a1c-135">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="18a1c-136">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="18a1c-136">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="18a1c-137">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="18a1c-137">groupLifetimeInDays</span></span>|<span data-ttu-id="18a1c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="18a1c-138">Int32</span></span>| <span data-ttu-id="18a1c-139">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="18a1c-139">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="18a1c-140">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="18a1c-140">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="18a1c-141">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="18a1c-141">managedGroupTypes</span></span>|<span data-ttu-id="18a1c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a1c-142">String</span></span>| <span data-ttu-id="18a1c-143">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="18a1c-143">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="18a1c-144">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="18a1c-144">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="18a1c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="18a1c-145">Response</span></span>

<span data-ttu-id="18a1c-146">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18a1c-146">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18a1c-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18a1c-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="18a1c-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18a1c-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="18a1c-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="18a1c-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="18a1c-150">C#</span><span class="sxs-lookup"><span data-stu-id="18a1c-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18a1c-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18a1c-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18a1c-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18a1c-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18a1c-153">Java</span><span class="sxs-lookup"><span data-stu-id="18a1c-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="18a1c-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="18a1c-154">Response</span></span>
<span data-ttu-id="18a1c-155">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="18a1c-155">Note: The response object shown here might be shortened for readability.</span></span> 
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

