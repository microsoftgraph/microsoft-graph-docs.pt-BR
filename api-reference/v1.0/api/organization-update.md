---
title: Atualize a organização
description: Atualize as propriedades da organização autenticada no momento.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 109c3f68e1eaa719f18a7fa8c539d09a2e3061aa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561408"
---
# <a name="update-organization"></a><span data-ttu-id="d0b7a-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="d0b7a-103">Update organization</span></span>

<span data-ttu-id="d0b7a-104">Atualize as propriedades da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="d0b7a-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="d0b7a-105">Nesse caso, `organization` é definido como uma coleção de exatamente um registro e, portanto, sua **ID** deve ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0b7a-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="d0b7a-106">O **ID** também é conhecido como **tenantid** da organização.</span><span class="sxs-lookup"><span data-stu-id="d0b7a-106">The **ID** is also known as the **tenantId** of the organization.</span></span>


## <a name="permissions"></a><span data-ttu-id="d0b7a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0b7a-107">Permissions</span></span>

<span data-ttu-id="d0b7a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0b7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0b7a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0b7a-110">Permission type</span></span> | <span data-ttu-id="d0b7a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0b7a-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0b7a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0b7a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0b7a-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0b7a-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0b7a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0b7a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0b7a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0b7a-115">Not supported.</span></span>    |
|<span data-ttu-id="d0b7a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0b7a-116">Application</span></span> | <span data-ttu-id="d0b7a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0b7a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0b7a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0b7a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}

```

## <a name="request-headers"></a><span data-ttu-id="d0b7a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0b7a-119">Request headers</span></span>

| <span data-ttu-id="d0b7a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d0b7a-120">Name</span></span>       | <span data-ttu-id="d0b7a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0b7a-121">Type</span></span> | <span data-ttu-id="d0b7a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0b7a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d0b7a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0b7a-123">Authorization</span></span>  | <span data-ttu-id="d0b7a-124">string</span><span class="sxs-lookup"><span data-stu-id="d0b7a-124">string</span></span>  | <span data-ttu-id="d0b7a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0b7a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0b7a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0b7a-127">Request body</span></span>

<span data-ttu-id="d0b7a-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d0b7a-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d0b7a-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d0b7a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d0b7a-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d0b7a-130">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d0b7a-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0b7a-131">Property</span></span>     | <span data-ttu-id="d0b7a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0b7a-132">Type</span></span>   |<span data-ttu-id="d0b7a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0b7a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0b7a-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="d0b7a-134">marketingNotificationEmails</span></span>|<span data-ttu-id="d0b7a-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0b7a-135">String collection</span></span>|                                        <span data-ttu-id="d0b7a-136">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="d0b7a-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="d0b7a-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="d0b7a-137">privacyProfile</span></span>|[<span data-ttu-id="d0b7a-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="d0b7a-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="d0b7a-139">O perfil de privacidade de uma organização (definir statementUrl e contactEmail).</span><span class="sxs-lookup"><span data-stu-id="d0b7a-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="d0b7a-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="d0b7a-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="d0b7a-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0b7a-141">String collection</span></span>||
|<span data-ttu-id="d0b7a-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="d0b7a-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="d0b7a-143">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0b7a-143">String collection</span></span>||
|<span data-ttu-id="d0b7a-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="d0b7a-144">technicalNotificationMails</span></span>|<span data-ttu-id="d0b7a-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0b7a-145">String collection</span></span>|                                        <span data-ttu-id="d0b7a-146">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="d0b7a-146">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="d0b7a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0b7a-147">Response</span></span>

<span data-ttu-id="d0b7a-148">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d0b7a-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d0b7a-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0b7a-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0b7a-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0b7a-150">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/{id}
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

### <a name="response"></a><span data-ttu-id="d0b7a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0b7a-151">Response</span></span>

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
