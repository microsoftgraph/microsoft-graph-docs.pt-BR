---
title: Atualize a organização
description: Atualize as propriedades da organização autenticada no momento.
ms.openlocfilehash: ac07f3ded31f8d6c7169d24208ed7e8cf967e07a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006611"
---
# <a name="update-organization"></a><span data-ttu-id="34b7e-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="34b7e-103">Update organization</span></span>

<span data-ttu-id="34b7e-104">Atualize as propriedades da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="34b7e-104">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="34b7e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="34b7e-105">Permissions</span></span>

<span data-ttu-id="34b7e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34b7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34b7e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34b7e-108">Permission type</span></span> | <span data-ttu-id="34b7e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34b7e-109">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34b7e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34b7e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34b7e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="34b7e-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="34b7e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34b7e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34b7e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34b7e-113">Not supported.</span></span>    |
|<span data-ttu-id="34b7e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34b7e-114">Application</span></span> | <span data-ttu-id="34b7e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34b7e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34b7e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34b7e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="34b7e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34b7e-117">Request headers</span></span>

| <span data-ttu-id="34b7e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="34b7e-118">Name</span></span>       | <span data-ttu-id="34b7e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="34b7e-119">Type</span></span> | <span data-ttu-id="34b7e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="34b7e-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="34b7e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="34b7e-121">Authorization</span></span>  | <span data-ttu-id="34b7e-122">string</span><span class="sxs-lookup"><span data-stu-id="34b7e-122">string</span></span>  | <span data-ttu-id="34b7e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34b7e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34b7e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34b7e-125">Request body</span></span>
<span data-ttu-id="34b7e-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="34b7e-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="34b7e-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="34b7e-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="34b7e-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="34b7e-128">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="34b7e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34b7e-129">Property</span></span>     | <span data-ttu-id="34b7e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="34b7e-130">Type</span></span>   |<span data-ttu-id="34b7e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="34b7e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34b7e-132">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="34b7e-132">marketingNotificationEmails</span></span>|<span data-ttu-id="34b7e-133">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34b7e-133">String collection</span></span>|                                        <span data-ttu-id="34b7e-134">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="34b7e-134">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="34b7e-135">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="34b7e-135">privacyProfile</span></span>|[<span data-ttu-id="34b7e-136">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="34b7e-136">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="34b7e-137">O perfil de privacidade de uma organização (definir statementUrl e contactEmail).</span><span class="sxs-lookup"><span data-stu-id="34b7e-137">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="34b7e-138">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="34b7e-138">securityComplianceNotificationMails</span></span>|<span data-ttu-id="34b7e-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="34b7e-139">String collection</span></span>||
|<span data-ttu-id="34b7e-140">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="34b7e-140">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="34b7e-141">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34b7e-141">String collection</span></span>||
|<span data-ttu-id="34b7e-142">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="34b7e-142">technicalNotificationMails</span></span>|<span data-ttu-id="34b7e-143">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34b7e-143">String collection</span></span>|                                        <span data-ttu-id="34b7e-144">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="34b7e-144">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="34b7e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="34b7e-145">Response</span></span>

<span data-ttu-id="34b7e-146">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="34b7e-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="34b7e-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34b7e-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="34b7e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34b7e-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
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

### <a name="response"></a><span data-ttu-id="34b7e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="34b7e-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
