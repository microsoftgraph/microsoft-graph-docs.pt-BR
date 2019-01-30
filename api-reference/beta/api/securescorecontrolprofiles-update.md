---
title: Atualizar secureScoreControlProfiles
description: Atualize uma propriedade editável secureScoreControlProfiles dentro de qualquer solução integrada para alterar várias propriedades, como assignedTo ou tenantNote.
localization_priority: Normal
ms.openlocfilehash: 711fd29e906822def0a5f4b5fbca13a1d73732d6
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642027"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="ac4e9-103">Atualizar secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="ac4e9-103">Update secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac4e9-104">Atualize uma propriedade editável **secureScoreControlProfiles** dentro de qualquer solução integrada para alterar várias propriedades, como **assignedTo** ou **tenantNote**.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-104">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac4e9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac4e9-105">Permissions</span></span>

<span data-ttu-id="ac4e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac4e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac4e9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac4e9-108">Permission type</span></span>      | <span data-ttu-id="ac4e9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac4e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac4e9-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac4e9-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="ac4e9-111">SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="ac4e9-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac4e9-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ac4e9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-113">Not supported.</span></span>  |
|<span data-ttu-id="ac4e9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac4e9-114">Application</span></span> | <span data-ttu-id="ac4e9-115">SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac4e9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac4e9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ac4e9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac4e9-117">Request headers</span></span>

| <span data-ttu-id="ac4e9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ac4e9-118">Name</span></span>       | <span data-ttu-id="ac4e9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac4e9-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ac4e9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac4e9-120">Authorization</span></span>  | <span data-ttu-id="ac4e9-p102">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-p102">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="ac4e9-123">Preferir</span><span class="sxs-lookup"><span data-stu-id="ac4e9-123">Prefer</span></span> | <span data-ttu-id="ac4e9-124">retornar = representação.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac4e9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac4e9-125">Request body</span></span>

<span data-ttu-id="ac4e9-126">No corpo da solicitação, fornece uma representação JSON dos valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ac4e9-127">A tabela a seguir lista os campos que podem ser atualizados por um secureScoreControlProfile.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-127">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="ac4e9-128">Os valores para propriedades existentes que não estão incluídos no corpo da solicitação não serão alterado.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-128">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="ac4e9-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ac4e9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac4e9-130">Property</span></span>   | <span data-ttu-id="ac4e9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac4e9-131">Type</span></span> |<span data-ttu-id="ac4e9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac4e9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac4e9-133">assignedTo</span><span class="sxs-lookup"><span data-stu-id="ac4e9-133">assignedTo</span></span>|<span data-ttu-id="ac4e9-134">String</span><span class="sxs-lookup"><span data-stu-id="ac4e9-134">String</span></span>|<span data-ttu-id="ac4e9-135">Nome do analista de controle é atribuída a triagem, implementação ou correção.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-135">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="ac4e9-136">tenantNote</span><span class="sxs-lookup"><span data-stu-id="ac4e9-136">tenantNote</span></span>|<span data-ttu-id="ac4e9-137">String</span><span class="sxs-lookup"><span data-stu-id="ac4e9-137">String</span></span>|<span data-ttu-id="ac4e9-138">Comentários de analistas no controle (para gerenciamento de controle do cliente).</span><span class="sxs-lookup"><span data-stu-id="ac4e9-138">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="ac4e9-139">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="ac4e9-139">controlStateUpdates</span></span>| <span data-ttu-id="ac4e9-140">String</span><span class="sxs-lookup"><span data-stu-id="ac4e9-140">String</span></span>|<span data-ttu-id="ac4e9-141">Analista orientada a configuração no controle.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-141">Analyst driven setting on the control.</span></span> <span data-ttu-id="ac4e9-142">Os valores possíveis são: `ignore`, `thirdParty`, `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-142">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="ac4e9-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac4e9-143">Response</span></span>

<span data-ttu-id="ac4e9-144">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-144">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="ac4e9-145">Se o cabeçalho de solicitação opcional for usado, o método retornará um `200 OK` código de resposta e o objeto atualizado [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-145">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac4e9-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac4e9-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac4e9-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac4e9-147">Request</span></span>

<span data-ttu-id="ac4e9-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-148">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ac4e9-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac4e9-149">Response</span></span>

<span data-ttu-id="ac4e9-150">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="ac4e9-150">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
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
    "Error: /api-reference/beta/api/securescorecontrolprofiles-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
