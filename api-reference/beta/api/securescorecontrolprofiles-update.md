---
title: Atualizar secureScoreControlProfiles
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: afbfcd1889c55dd53241ff8d796bb3ab492b2acf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033134"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="c2178-104">Atualizar secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="c2178-104">Update secureScoreControlProfiles</span></span>

 > <span data-ttu-id="c2178-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c2178-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2178-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c2178-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2178-107">Atualize uma propriedade editável **secureScoreControlProfiles** dentro de qualquer solução integrada para alterar várias propriedades, como **assignedTo** ou **tenantNote**.</span><span class="sxs-lookup"><span data-stu-id="c2178-107">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2178-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="c2178-108">Permissions</span></span>

<span data-ttu-id="c2178-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2178-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2178-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2178-111">Permission type</span></span>      | <span data-ttu-id="c2178-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2178-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2178-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2178-113">Delegated (work or school account)</span></span> |   <span data-ttu-id="c2178-114">SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="c2178-114">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="c2178-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2178-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c2178-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2178-116">Not supported.</span></span>  |
|<span data-ttu-id="c2178-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2178-117">Application</span></span> | <span data-ttu-id="c2178-118">SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="c2178-118">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2178-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2178-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c2178-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2178-120">Request headers</span></span>

| <span data-ttu-id="c2178-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c2178-121">Name</span></span>       | <span data-ttu-id="c2178-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2178-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c2178-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2178-123">Authorization</span></span>  | <span data-ttu-id="c2178-p104">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2178-p104">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="c2178-126">Preferir</span><span class="sxs-lookup"><span data-stu-id="c2178-126">Prefer</span></span> | <span data-ttu-id="c2178-127">retornar = representação.</span><span class="sxs-lookup"><span data-stu-id="c2178-127">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2178-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2178-128">Request body</span></span>

<span data-ttu-id="c2178-129">No corpo da solicitação, fornece uma representação JSON dos valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="c2178-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c2178-130">A tabela a seguir lista os campos que podem ser atualizados por um secureScoreControlProfile.</span><span class="sxs-lookup"><span data-stu-id="c2178-130">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="c2178-131">Os valores para propriedades existentes que não estão incluídos no corpo da solicitação não serão alterado.</span><span class="sxs-lookup"><span data-stu-id="c2178-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="c2178-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c2178-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c2178-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2178-133">Property</span></span>   | <span data-ttu-id="c2178-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2178-134">Type</span></span> |<span data-ttu-id="c2178-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2178-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2178-136">assignedTo</span><span class="sxs-lookup"><span data-stu-id="c2178-136">assignedTo</span></span>|<span data-ttu-id="c2178-137">String</span><span class="sxs-lookup"><span data-stu-id="c2178-137">String</span></span>|<span data-ttu-id="c2178-138">Nome do analista de controle é atribuída a triagem, implementação ou correção.</span><span class="sxs-lookup"><span data-stu-id="c2178-138">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="c2178-139">tenantNote</span><span class="sxs-lookup"><span data-stu-id="c2178-139">tenantNote</span></span>|<span data-ttu-id="c2178-140">String</span><span class="sxs-lookup"><span data-stu-id="c2178-140">String</span></span>|<span data-ttu-id="c2178-141">Comentários de analistas no controle (para gerenciamento de controle do cliente).</span><span class="sxs-lookup"><span data-stu-id="c2178-141">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="c2178-142">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="c2178-142">controlStateUpdates</span></span>| <span data-ttu-id="c2178-143">String</span><span class="sxs-lookup"><span data-stu-id="c2178-143">String</span></span>|<span data-ttu-id="c2178-144">Analista orientada a configuração no controle.</span><span class="sxs-lookup"><span data-stu-id="c2178-144">Analyst driven setting on the control.</span></span> <span data-ttu-id="c2178-145">Os valores possíveis são: `ignore`, `thirdParty`, `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="c2178-145">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="c2178-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2178-146">Response</span></span>

<span data-ttu-id="c2178-147">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c2178-147">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="c2178-148">Se o cabeçalho de solicitação opcional for usado, o método retornará um `200 OK` código de resposta e o objeto atualizado [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2178-148">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2178-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2178-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2178-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2178-150">Request</span></span>

<span data-ttu-id="c2178-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2178-151">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "assignedTo": "assignedTo-value",
  "controlStateUpdates": "controlStateUpdates-value",
  "tenantNote": "tenantNote-value"
}
```

### <a name="response"></a><span data-ttu-id="c2178-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2178-152">Response</span></span>

<span data-ttu-id="c2178-153">O exemplo a seguir é um exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="c2178-153">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```




<!-- {
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
