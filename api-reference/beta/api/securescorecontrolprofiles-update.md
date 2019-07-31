---
title: Atualizar secureScoreControlProfiles
description: Atualize uma propriedade secureScoreControlProfiles editável em qualquer solução integrada para alterar várias propriedades, como assignedTo ou tenantNote.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3450422320cf1d80bdd4cfd2f7e67960c0bafdbc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978040"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="bbb9a-103">Atualizar secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="bbb9a-103">Update secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbb9a-104">Atualize uma propriedade **secureScoreControlProfiles** editável em qualquer solução integrada para alterar várias propriedades, como **assignedTo** ou **tenantNote**.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-104">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbb9a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbb9a-105">Permissions</span></span>

<span data-ttu-id="bbb9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbb9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbb9a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbb9a-108">Permission type</span></span>      | <span data-ttu-id="bbb9a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbb9a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbb9a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbb9a-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="bbb9a-111">Escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="bbb9a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbb9a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bbb9a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-113">Not supported.</span></span>  |
|<span data-ttu-id="bbb9a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbb9a-114">Application</span></span> | <span data-ttu-id="bbb9a-115">Escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbb9a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbb9a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bbb9a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9a-117">Request headers</span></span>

| <span data-ttu-id="bbb9a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bbb9a-118">Name</span></span>       | <span data-ttu-id="bbb9a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bbb9a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbb9a-120">Authorization</span></span>  | <span data-ttu-id="bbb9a-121">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-121">Bearer {code}.</span></span> <span data-ttu-id="bbb9a-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-122">Required.</span></span>|
|<span data-ttu-id="bbb9a-123">Preferir</span><span class="sxs-lookup"><span data-stu-id="bbb9a-123">Prefer</span></span> | <span data-ttu-id="bbb9a-124">Return = representação.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbb9a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9a-125">Request body</span></span>

<span data-ttu-id="bbb9a-126">No corpo da solicitação, forneça uma representação JSON dos valores de campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bbb9a-127">A tabela a seguir lista os campos que podem ser atualizados para um secureScoreControlProfile.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-127">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="bbb9a-128">Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-128">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="bbb9a-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bbb9a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbb9a-130">Property</span></span>   | <span data-ttu-id="bbb9a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbb9a-131">Type</span></span> |<span data-ttu-id="bbb9a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb9a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbb9a-133">assignedTo</span><span class="sxs-lookup"><span data-stu-id="bbb9a-133">assignedTo</span></span>|<span data-ttu-id="bbb9a-134">String</span><span class="sxs-lookup"><span data-stu-id="bbb9a-134">String</span></span>|<span data-ttu-id="bbb9a-135">Nome do analista ao qual o controle é atribuído para a triagem, implementação ou correção.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-135">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="bbb9a-136">tenantNote</span><span class="sxs-lookup"><span data-stu-id="bbb9a-136">tenantNote</span></span>|<span data-ttu-id="bbb9a-137">String</span><span class="sxs-lookup"><span data-stu-id="bbb9a-137">String</span></span>|<span data-ttu-id="bbb9a-138">Comentários de analista sobre o controle (para o gerenciamento de controle de clientes).</span><span class="sxs-lookup"><span data-stu-id="bbb9a-138">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="bbb9a-139">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="bbb9a-139">controlStateUpdates</span></span>| <span data-ttu-id="bbb9a-140">String</span><span class="sxs-lookup"><span data-stu-id="bbb9a-140">String</span></span>|<span data-ttu-id="bbb9a-141">Configuração orientada pelo analista no controle.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-141">Analyst driven setting on the control.</span></span> <span data-ttu-id="bbb9a-142">Os valores possíveis são: `ignore`, `thirdParty`, `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-142">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="bbb9a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbb9a-143">Response</span></span>

<span data-ttu-id="bbb9a-144">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-144">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="bbb9a-145">Se o cabeçalho de solicitação opcional for usado, o método retornará `200 OK` um código de resposta e o objeto [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-145">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbb9a-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbb9a-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbb9a-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb9a-147">Request</span></span>

<span data-ttu-id="bbb9a-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-148">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bbb9a-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbb9a-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bbb9a-150">C#</span><span class="sxs-lookup"><span data-stu-id="bbb9a-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bbb9a-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="bbb9a-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bbb9a-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bbb9a-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bbb9a-153">Java</span><span class="sxs-lookup"><span data-stu-id="bbb9a-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securescorecontrolprofiles-update-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bbb9a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbb9a-154">Response</span></span>

<span data-ttu-id="bbb9a-155">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-155">The following is an example of a successful response.</span></span>
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
