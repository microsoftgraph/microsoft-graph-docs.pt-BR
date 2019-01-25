---
title: Atualizar privilegedapproval
description: Atualize as propriedades do objeto privilegedapproval.
localization_priority: Normal
ms.openlocfilehash: cb108ca35b07138f84a9fd969bfe7c7241e9672e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524895"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="eb189-103">Atualizar privilegedapproval</span><span class="sxs-lookup"><span data-stu-id="eb189-103">Update privilegedapproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb189-104">Atualize as propriedades do objeto privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="eb189-104">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb189-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb189-105">Permissions</span></span>
<span data-ttu-id="eb189-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb189-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eb189-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb189-108">Permission type</span></span>      | <span data-ttu-id="eb189-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb189-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb189-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb189-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eb189-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eb189-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eb189-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb189-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb189-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb189-113">Not supported.</span></span>    |
|<span data-ttu-id="eb189-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb189-114">Application</span></span> | <span data-ttu-id="eb189-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb189-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb189-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb189-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="eb189-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="eb189-117">Optional request headers</span></span>
| <span data-ttu-id="eb189-118">Nome</span><span class="sxs-lookup"><span data-stu-id="eb189-118">Name</span></span>       | <span data-ttu-id="eb189-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb189-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="eb189-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb189-120">Authorization</span></span>  | <span data-ttu-id="eb189-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb189-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb189-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb189-123">Request body</span></span>
<span data-ttu-id="eb189-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="eb189-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eb189-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb189-127">Property</span></span>     | <span data-ttu-id="eb189-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb189-128">Type</span></span>   |<span data-ttu-id="eb189-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb189-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb189-130">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="eb189-130">approvalDuration</span></span>|<span data-ttu-id="eb189-131">Duration</span><span class="sxs-lookup"><span data-stu-id="eb189-131">Duration</span></span>||
|<span data-ttu-id="eb189-132">approvalState</span><span class="sxs-lookup"><span data-stu-id="eb189-132">approvalState</span></span>|<span data-ttu-id="eb189-133">string</span><span class="sxs-lookup"><span data-stu-id="eb189-133">string</span></span>| <span data-ttu-id="eb189-134">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="eb189-134">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="eb189-135">approvalType</span><span class="sxs-lookup"><span data-stu-id="eb189-135">approvalType</span></span>|<span data-ttu-id="eb189-136">String</span><span class="sxs-lookup"><span data-stu-id="eb189-136">String</span></span>||
|<span data-ttu-id="eb189-137">approverReason</span><span class="sxs-lookup"><span data-stu-id="eb189-137">approverReason</span></span>|<span data-ttu-id="eb189-138">String</span><span class="sxs-lookup"><span data-stu-id="eb189-138">String</span></span>||
|<span data-ttu-id="eb189-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="eb189-139">endDateTime</span></span>|<span data-ttu-id="eb189-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb189-140">DateTimeOffset</span></span>||
|<span data-ttu-id="eb189-141">requestorReason</span><span class="sxs-lookup"><span data-stu-id="eb189-141">requestorReason</span></span>|<span data-ttu-id="eb189-142">String</span><span class="sxs-lookup"><span data-stu-id="eb189-142">String</span></span>||
|<span data-ttu-id="eb189-143">roleId</span><span class="sxs-lookup"><span data-stu-id="eb189-143">roleId</span></span>|<span data-ttu-id="eb189-144">String</span><span class="sxs-lookup"><span data-stu-id="eb189-144">String</span></span>||
|<span data-ttu-id="eb189-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="eb189-145">startDateTime</span></span>|<span data-ttu-id="eb189-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb189-146">DateTimeOffset</span></span>||
|<span data-ttu-id="eb189-147">userId</span><span class="sxs-lookup"><span data-stu-id="eb189-147">userId</span></span>|<span data-ttu-id="eb189-148">String</span><span class="sxs-lookup"><span data-stu-id="eb189-148">String</span></span>||

## <a name="response"></a><span data-ttu-id="eb189-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb189-149">Response</span></span>

<span data-ttu-id="eb189-150">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eb189-150">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="eb189-151">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="eb189-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="eb189-152">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="eb189-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="eb189-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb189-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb189-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb189-154">Request</span></span>
<span data-ttu-id="eb189-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb189-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedApproval{request-id}
Content-type: application/json
Content-length: 180

{
  "approvalState": "approvalState-value",
  "approverReason": "approverReason-value"
}
```
##### <a name="response"></a><span data-ttu-id="eb189-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb189-156">Response</span></span>
<span data-ttu-id="eb189-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb189-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedapproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
