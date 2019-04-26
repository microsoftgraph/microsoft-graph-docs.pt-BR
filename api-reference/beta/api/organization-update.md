---
title: Atualize a organização
description: Atualize as propriedades da organização autenticada no momento.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0c60ef631177431350a896c77bbe1dab80f7b985
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338086"
---
# <a name="update-organization"></a><span data-ttu-id="367d9-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="367d9-103">Update organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="367d9-104">Atualize as propriedades da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="367d9-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="367d9-105">Nesse caso, `organization` é definido como uma coleção de exatamente um registro e, portanto, sua **ID** deve ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="367d9-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="367d9-106">O **ID** também é conhecido como **tenantid** da organização.</span><span class="sxs-lookup"><span data-stu-id="367d9-106">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="367d9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="367d9-107">Permissions</span></span>

<span data-ttu-id="367d9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="367d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="367d9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="367d9-110">Permission type</span></span> | <span data-ttu-id="367d9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="367d9-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="367d9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="367d9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="367d9-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="367d9-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="367d9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="367d9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="367d9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="367d9-115">Not supported.</span></span> |
|<span data-ttu-id="367d9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="367d9-116">Application</span></span> | <span data-ttu-id="367d9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="367d9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="367d9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="367d9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="367d9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="367d9-119">Request headers</span></span>

| <span data-ttu-id="367d9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="367d9-120">Name</span></span>       | <span data-ttu-id="367d9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="367d9-121">Type</span></span> | <span data-ttu-id="367d9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="367d9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="367d9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="367d9-123">Authorization</span></span>  | <span data-ttu-id="367d9-124">string</span><span class="sxs-lookup"><span data-stu-id="367d9-124">string</span></span>  | <span data-ttu-id="367d9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="367d9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="367d9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="367d9-127">Request body</span></span>

<span data-ttu-id="367d9-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="367d9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="367d9-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="367d9-131">Property</span></span>     | <span data-ttu-id="367d9-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="367d9-132">Type</span></span>   |<span data-ttu-id="367d9-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="367d9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="367d9-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="367d9-134">marketingNotificationEmails</span></span>|<span data-ttu-id="367d9-135">Coleção String</span><span class="sxs-lookup"><span data-stu-id="367d9-135">String collection</span></span>|                                        <span data-ttu-id="367d9-136">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="367d9-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="367d9-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="367d9-137">privacyProfile</span></span>|[<span data-ttu-id="367d9-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="367d9-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="367d9-139">O perfil de privacidade de uma organização (definir statementUrl e contactEmail).</span><span class="sxs-lookup"><span data-stu-id="367d9-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="367d9-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="367d9-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="367d9-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="367d9-141">String collection</span></span>||
|<span data-ttu-id="367d9-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="367d9-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="367d9-143">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="367d9-143">String collection</span></span>||
|<span data-ttu-id="367d9-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="367d9-144">technicalNotificationMails</span></span>|<span data-ttu-id="367d9-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="367d9-145">String collection</span></span>|                                        <span data-ttu-id="367d9-146">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="367d9-146">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="367d9-147">Como o recurso de **organização** oferece suporte a [extensões](/graph/extensibility-overview), você `PATCH` pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância de **organização** existente.</span><span class="sxs-lookup"><span data-stu-id="367d9-147">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="367d9-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="367d9-148">Response</span></span>

<span data-ttu-id="367d9-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="367d9-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="367d9-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="367d9-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="367d9-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="367d9-152">Request</span></span>
<span data-ttu-id="367d9-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="367d9-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{id}
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

##### <a name="response"></a><span data-ttu-id="367d9-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="367d9-154">Response</span></span>

<span data-ttu-id="367d9-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="367d9-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="367d9-156">Confira também</span><span class="sxs-lookup"><span data-stu-id="367d9-156">See also</span></span>

- [<span data-ttu-id="367d9-157">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="367d9-157">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="367d9-158">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="367d9-158">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
