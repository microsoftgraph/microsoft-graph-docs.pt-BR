---
title: Atualizar secureScoreControlProfiles
description: Atualize uma propriedade secureScoreControlProfiles editável em qualquer solução integrada para alterar várias propriedades, como assignedTo ou tenantNote.
localization_priority: Normal
ms.openlocfilehash: 711fd29e906822def0a5f4b5fbca13a1d73732d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545563"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="17141-103">Atualizar secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="17141-103">Update secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17141-104">Atualize uma propriedade **secureScoreControlProfiles** editável em qualquer solução integrada para alterar várias propriedades, como **assignedTo** ou **tenantNote**.</span><span class="sxs-lookup"><span data-stu-id="17141-104">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="17141-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="17141-105">Permissions</span></span>

<span data-ttu-id="17141-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17141-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17141-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17141-108">Permission type</span></span>      | <span data-ttu-id="17141-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17141-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17141-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17141-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="17141-111">Escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="17141-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="17141-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17141-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="17141-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17141-113">Not supported.</span></span>  |
|<span data-ttu-id="17141-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17141-114">Application</span></span> | <span data-ttu-id="17141-115">Escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="17141-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17141-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17141-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="17141-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17141-117">Request headers</span></span>

| <span data-ttu-id="17141-118">Nome</span><span class="sxs-lookup"><span data-stu-id="17141-118">Name</span></span>       | <span data-ttu-id="17141-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="17141-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="17141-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="17141-120">Authorization</span></span>  | <span data-ttu-id="17141-121">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="17141-121">Bearer {code}.</span></span> <span data-ttu-id="17141-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17141-122">Required.</span></span>|
|<span data-ttu-id="17141-123">Preferir</span><span class="sxs-lookup"><span data-stu-id="17141-123">Prefer</span></span> | <span data-ttu-id="17141-124">Return = representação.</span><span class="sxs-lookup"><span data-stu-id="17141-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17141-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17141-125">Request body</span></span>

<span data-ttu-id="17141-126">No corpo da solicitação, forneça uma representação JSON dos valores de campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="17141-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="17141-127">A tabela a seguir lista os campos que podem ser atualizados para um secureScoreControlProfile.</span><span class="sxs-lookup"><span data-stu-id="17141-127">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="17141-128">Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados.</span><span class="sxs-lookup"><span data-stu-id="17141-128">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="17141-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="17141-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="17141-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17141-130">Property</span></span>   | <span data-ttu-id="17141-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="17141-131">Type</span></span> |<span data-ttu-id="17141-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="17141-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17141-133">assignedTo</span><span class="sxs-lookup"><span data-stu-id="17141-133">assignedTo</span></span>|<span data-ttu-id="17141-134">String</span><span class="sxs-lookup"><span data-stu-id="17141-134">String</span></span>|<span data-ttu-id="17141-135">Nome do analista ao qual o controle é atribuído para a triagem, implementação ou correção.</span><span class="sxs-lookup"><span data-stu-id="17141-135">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="17141-136">tenantNote</span><span class="sxs-lookup"><span data-stu-id="17141-136">tenantNote</span></span>|<span data-ttu-id="17141-137">String</span><span class="sxs-lookup"><span data-stu-id="17141-137">String</span></span>|<span data-ttu-id="17141-138">Comentários de analista sobre o controle (para o gerenciamento de controle de clientes).</span><span class="sxs-lookup"><span data-stu-id="17141-138">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="17141-139">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="17141-139">controlStateUpdates</span></span>| <span data-ttu-id="17141-140">String</span><span class="sxs-lookup"><span data-stu-id="17141-140">String</span></span>|<span data-ttu-id="17141-141">Configuração orientada pelo analista no controle.</span><span class="sxs-lookup"><span data-stu-id="17141-141">Analyst driven setting on the control.</span></span> <span data-ttu-id="17141-142">Os valores possíveis são: `ignore`, `thirdParty`, `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="17141-142">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="17141-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="17141-143">Response</span></span>

<span data-ttu-id="17141-144">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="17141-144">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="17141-145">Se o cabeçalho de solicitação opcional for usado, o método retornará `200 OK` um código de resposta e o objeto [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17141-145">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17141-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17141-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="17141-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17141-147">Request</span></span>

<span data-ttu-id="17141-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="17141-148">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="17141-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="17141-149">Response</span></span>

<span data-ttu-id="17141-150">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="17141-150">The following is an example of a successful response.</span></span>
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
