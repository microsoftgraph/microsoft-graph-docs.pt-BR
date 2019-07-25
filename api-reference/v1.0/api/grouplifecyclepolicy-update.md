---
title: Atualizar groupLifecyclePolicy
description: Atualiza as propriedades de um objeto do tipo de recurso groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 1e75863416faddfaf2a00287a03d2df801259c25
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886800"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="a82ad-103">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a82ad-103">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="a82ad-104">Atualiza as propriedades de um objeto do [tipo de recurso groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a82ad-104">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a82ad-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a82ad-105">Permissions</span></span>

<span data-ttu-id="a82ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a82ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 
|<span data-ttu-id="a82ad-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a82ad-108">Permission type</span></span>      | <span data-ttu-id="a82ad-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a82ad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a82ad-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a82ad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a82ad-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a82ad-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a82ad-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a82ad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a82ad-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a82ad-113">Not supported.</span></span>    |
|<span data-ttu-id="a82ad-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a82ad-114">Application</span></span> | <span data-ttu-id="a82ad-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a82ad-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a82ad-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a82ad-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="a82ad-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="a82ad-117">Optional request headers</span></span>
| <span data-ttu-id="a82ad-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a82ad-118">Name</span></span> | <span data-ttu-id="a82ad-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a82ad-119">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="a82ad-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a82ad-120">Authorization</span></span> | <span data-ttu-id="a82ad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a82ad-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a82ad-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a82ad-123">Content-Type</span></span>  | <span data-ttu-id="a82ad-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a82ad-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a82ad-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a82ad-125">Request body</span></span>

<span data-ttu-id="a82ad-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a82ad-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a82ad-127">As propriedades existentes que não estão incluídas no corpo da solicitação mantêm os valores anteriores ou recalcula-os com base nas alterações feitas em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a82ad-127">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="a82ad-128">Para obter o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a82ad-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a82ad-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a82ad-129">Property</span></span> | <span data-ttu-id="a82ad-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a82ad-130">Type</span></span> | <span data-ttu-id="a82ad-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a82ad-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a82ad-132">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="a82ad-132">alternateNotificationEmails</span></span>|<span data-ttu-id="a82ad-133">String</span><span class="sxs-lookup"><span data-stu-id="a82ad-133">String</span></span>| <span data-ttu-id="a82ad-134">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="a82ad-134">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="a82ad-135">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="a82ad-135">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="a82ad-136">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="a82ad-136">groupLifetimeInDays</span></span>|<span data-ttu-id="a82ad-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a82ad-137">Int32</span></span>| <span data-ttu-id="a82ad-138">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="a82ad-138">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="a82ad-139">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="a82ad-139">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="a82ad-140">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="a82ad-140">managedGroupTypes</span></span>|<span data-ttu-id="a82ad-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a82ad-141">String</span></span>| <span data-ttu-id="a82ad-142">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="a82ad-142">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="a82ad-143">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="a82ad-143">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="a82ad-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a82ad-144">Response</span></span>

<span data-ttu-id="a82ad-145">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a82ad-145">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a82ad-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a82ad-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a82ad-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a82ad-147">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a82ad-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="a82ad-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a82ad-149">C#</span><span class="sxs-lookup"><span data-stu-id="a82ad-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a82ad-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="a82ad-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a82ad-151">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a82ad-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a82ad-152">Java</span><span class="sxs-lookup"><span data-stu-id="a82ad-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a82ad-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a82ad-153">Response</span></span>
<span data-ttu-id="a82ad-154">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a82ad-154">Note: The response object shown here may be truncated for brevity.</span></span> 
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
