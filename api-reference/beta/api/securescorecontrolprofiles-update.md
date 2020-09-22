---
title: Atualizar secureScoreControlProfiles
description: Atualize uma propriedade secureScoreControlProfiles editável em qualquer solução integrada para alterar várias propriedades, como assignedTo ou tenantNote.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: eaa11591f5174f8d77e9513cb9bba3ed1de44976
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067535"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="f1fcb-103">Atualizar secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="f1fcb-103">Update secureScoreControlProfiles</span></span>

<span data-ttu-id="f1fcb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1fcb-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1fcb-105">Atualize uma propriedade **secureScoreControlProfiles** editável em qualquer solução integrada para alterar várias propriedades, como **assignedTo** ou **tenantNote**.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-105">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1fcb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1fcb-106">Permissions</span></span>

<span data-ttu-id="f1fcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1fcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1fcb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1fcb-109">Permission type</span></span>      | <span data-ttu-id="f1fcb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1fcb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1fcb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1fcb-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="f1fcb-112">Escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-112">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="f1fcb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1fcb-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f1fcb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-114">Not supported.</span></span>  |
|<span data-ttu-id="f1fcb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1fcb-115">Application</span></span> | <span data-ttu-id="f1fcb-116">Escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-116">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1fcb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1fcb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f1fcb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1fcb-118">Request headers</span></span>

| <span data-ttu-id="f1fcb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f1fcb-119">Name</span></span>       | <span data-ttu-id="f1fcb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1fcb-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f1fcb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1fcb-121">Authorization</span></span>  | <span data-ttu-id="f1fcb-122">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-122">Bearer {code}.</span></span> <span data-ttu-id="f1fcb-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-123">Required.</span></span>|
|<span data-ttu-id="f1fcb-124">Preferir</span><span class="sxs-lookup"><span data-stu-id="f1fcb-124">Prefer</span></span> | <span data-ttu-id="f1fcb-125">Return = representação.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-125">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1fcb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1fcb-126">Request body</span></span>

<span data-ttu-id="f1fcb-127">No corpo da solicitação, forneça uma representação JSON dos valores de campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-127">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f1fcb-128">A tabela a seguir lista os campos que podem ser atualizados para um secureScoreControlProfile.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-128">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="f1fcb-129">Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="f1fcb-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f1fcb-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1fcb-131">Property</span></span>   | <span data-ttu-id="f1fcb-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1fcb-132">Type</span></span> |<span data-ttu-id="f1fcb-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1fcb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1fcb-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="f1fcb-134">assignedTo</span></span>|<span data-ttu-id="f1fcb-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1fcb-135">String</span></span>|<span data-ttu-id="f1fcb-136">Nome do analista ao qual o controle é atribuído para a triagem, implementação ou correção.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-136">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="f1fcb-137">tenantNote</span><span class="sxs-lookup"><span data-stu-id="f1fcb-137">tenantNote</span></span>|<span data-ttu-id="f1fcb-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1fcb-138">String</span></span>|<span data-ttu-id="f1fcb-139">Comentários de analista sobre o controle (para o gerenciamento de controle de clientes).</span><span class="sxs-lookup"><span data-stu-id="f1fcb-139">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="f1fcb-140">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="f1fcb-140">controlStateUpdates</span></span>| <span data-ttu-id="f1fcb-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1fcb-141">String</span></span>|<span data-ttu-id="f1fcb-142">Configuração orientada pelo analista no controle.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-142">Analyst driven setting on the control.</span></span> <span data-ttu-id="f1fcb-143">Os valores possíveis são: `ignore`, `thirdParty`, `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-143">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="f1fcb-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1fcb-144">Response</span></span>

<span data-ttu-id="f1fcb-145">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-145">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="f1fcb-146">Se o cabeçalho de solicitação opcional for usado, o método retornará um `200 OK` código de resposta e o objeto [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-146">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1fcb-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1fcb-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1fcb-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1fcb-148">Request</span></span>

<span data-ttu-id="f1fcb-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1fcb-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1fcb-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "controlStateUpdates": "controlStateUpdates-value"
}
```
# <a name="c"></a>[<span data-ttu-id="f1fcb-151">C#</span><span class="sxs-lookup"><span data-stu-id="f1fcb-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1fcb-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1fcb-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1fcb-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1fcb-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1fcb-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1fcb-154">Response</span></span>

<span data-ttu-id="f1fcb-155">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="f1fcb-155">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 204 No Content
```




<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


