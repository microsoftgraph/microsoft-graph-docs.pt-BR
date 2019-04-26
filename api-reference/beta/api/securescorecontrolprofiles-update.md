---
title: Atualizar secureScoreControlProfiles
description: Atualize uma propriedade secureScoreControlProfiles editável em qualquer solução integrada para alterar várias propriedades, como assignedTo ou tenantNote.
localization_priority: Normal
ms.openlocfilehash: ee184e921301fc8e2ce9e86122e5f01c335fa540
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331458"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="c0620-103">Atualizar secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="c0620-103">Update secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0620-104">Atualize uma propriedade **secureScoreControlProfiles** editável em qualquer solução integrada para alterar várias propriedades, como **assignedTo** ou **tenantNote**.</span><span class="sxs-lookup"><span data-stu-id="c0620-104">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0620-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0620-105">Permissions</span></span>

<span data-ttu-id="c0620-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0620-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0620-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0620-108">Permission type</span></span>      | <span data-ttu-id="c0620-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0620-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0620-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0620-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="c0620-111">Escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="c0620-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="c0620-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0620-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c0620-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0620-113">Not supported.</span></span>  |
|<span data-ttu-id="c0620-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0620-114">Application</span></span> | <span data-ttu-id="c0620-115">Escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="c0620-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0620-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0620-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c0620-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0620-117">Request headers</span></span>

| <span data-ttu-id="c0620-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c0620-118">Name</span></span>       | <span data-ttu-id="c0620-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0620-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c0620-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0620-120">Authorization</span></span>  | <span data-ttu-id="c0620-121">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="c0620-121">Bearer {code}.</span></span> <span data-ttu-id="c0620-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0620-122">Required.</span></span>|
|<span data-ttu-id="c0620-123">Preferir</span><span class="sxs-lookup"><span data-stu-id="c0620-123">Prefer</span></span> | <span data-ttu-id="c0620-124">Return = representação.</span><span class="sxs-lookup"><span data-stu-id="c0620-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0620-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0620-125">Request body</span></span>

<span data-ttu-id="c0620-126">No corpo da solicitação, forneça uma representação JSON dos valores de campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="c0620-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c0620-127">A tabela a seguir lista os campos que podem ser atualizados para um secureScoreControlProfile.</span><span class="sxs-lookup"><span data-stu-id="c0620-127">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="c0620-128">Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados.</span><span class="sxs-lookup"><span data-stu-id="c0620-128">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="c0620-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c0620-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c0620-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0620-130">Property</span></span>   | <span data-ttu-id="c0620-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0620-131">Type</span></span> |<span data-ttu-id="c0620-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0620-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0620-133">assignedTo</span><span class="sxs-lookup"><span data-stu-id="c0620-133">assignedTo</span></span>|<span data-ttu-id="c0620-134">String</span><span class="sxs-lookup"><span data-stu-id="c0620-134">String</span></span>|<span data-ttu-id="c0620-135">Nome do analista ao qual o controle é atribuído para a triagem, implementação ou correção.</span><span class="sxs-lookup"><span data-stu-id="c0620-135">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="c0620-136">tenantNote</span><span class="sxs-lookup"><span data-stu-id="c0620-136">tenantNote</span></span>|<span data-ttu-id="c0620-137">String</span><span class="sxs-lookup"><span data-stu-id="c0620-137">String</span></span>|<span data-ttu-id="c0620-138">Comentários de analista sobre o controle (para o gerenciamento de controle de clientes).</span><span class="sxs-lookup"><span data-stu-id="c0620-138">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="c0620-139">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="c0620-139">controlStateUpdates</span></span>| <span data-ttu-id="c0620-140">String</span><span class="sxs-lookup"><span data-stu-id="c0620-140">String</span></span>|<span data-ttu-id="c0620-141">Configuração orientada pelo analista no controle.</span><span class="sxs-lookup"><span data-stu-id="c0620-141">Analyst driven setting on the control.</span></span> <span data-ttu-id="c0620-142">Os valores possíveis são: `ignore`, `thirdParty`, `reviewed`.</span><span class="sxs-lookup"><span data-stu-id="c0620-142">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="c0620-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0620-143">Response</span></span>

<span data-ttu-id="c0620-144">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c0620-144">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="c0620-145">Se o cabeçalho de solicitação opcional for usado, o método retornará `200 OK` um código de resposta e o objeto [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0620-145">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0620-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0620-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0620-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0620-147">Request</span></span>

<span data-ttu-id="c0620-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0620-148">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c0620-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0620-149">Response</span></span>

<span data-ttu-id="c0620-150">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="c0620-150">The following is an example of a successful response.</span></span>
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
  "suppressions": []
}
-->
