---
title: Atualizar privilegedapproval
description: Atualize as propriedades do objeto privilegedapproval.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6103e01ea9832bd7858215576eaeb4319514d6be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978802"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="29747-103">Atualizar privilegedapproval</span><span class="sxs-lookup"><span data-stu-id="29747-103">Update privilegedapproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29747-104">Atualize as propriedades do objeto privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="29747-104">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="29747-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="29747-105">Permissions</span></span>
<span data-ttu-id="29747-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29747-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="29747-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29747-108">Permission type</span></span>      | <span data-ttu-id="29747-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29747-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29747-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29747-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29747-111">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="29747-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29747-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29747-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29747-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29747-113">Not supported.</span></span>    |
|<span data-ttu-id="29747-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29747-114">Application</span></span> | <span data-ttu-id="29747-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29747-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29747-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29747-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="29747-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="29747-117">Optional request headers</span></span>
| <span data-ttu-id="29747-118">Nome</span><span class="sxs-lookup"><span data-stu-id="29747-118">Name</span></span>       | <span data-ttu-id="29747-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="29747-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="29747-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="29747-120">Authorization</span></span>  | <span data-ttu-id="29747-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29747-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29747-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29747-123">Request body</span></span>
<span data-ttu-id="29747-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="29747-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="29747-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29747-127">Property</span></span>     | <span data-ttu-id="29747-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="29747-128">Type</span></span>   |<span data-ttu-id="29747-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="29747-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29747-130">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="29747-130">approvalDuration</span></span>|<span data-ttu-id="29747-131">Duração</span><span class="sxs-lookup"><span data-stu-id="29747-131">Duration</span></span>||
|<span data-ttu-id="29747-132">approvalstate</span><span class="sxs-lookup"><span data-stu-id="29747-132">approvalState</span></span>|<span data-ttu-id="29747-133">string</span><span class="sxs-lookup"><span data-stu-id="29747-133">string</span></span>| <span data-ttu-id="29747-134">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="29747-134">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="29747-135">approvaltype</span><span class="sxs-lookup"><span data-stu-id="29747-135">approvalType</span></span>|<span data-ttu-id="29747-136">String</span><span class="sxs-lookup"><span data-stu-id="29747-136">String</span></span>||
|<span data-ttu-id="29747-137">approverReason</span><span class="sxs-lookup"><span data-stu-id="29747-137">approverReason</span></span>|<span data-ttu-id="29747-138">String</span><span class="sxs-lookup"><span data-stu-id="29747-138">String</span></span>||
|<span data-ttu-id="29747-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="29747-139">endDateTime</span></span>|<span data-ttu-id="29747-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29747-140">DateTimeOffset</span></span>||
|<span data-ttu-id="29747-141">requestorReason</span><span class="sxs-lookup"><span data-stu-id="29747-141">requestorReason</span></span>|<span data-ttu-id="29747-142">String</span><span class="sxs-lookup"><span data-stu-id="29747-142">String</span></span>||
|<span data-ttu-id="29747-143">roleId</span><span class="sxs-lookup"><span data-stu-id="29747-143">roleId</span></span>|<span data-ttu-id="29747-144">String</span><span class="sxs-lookup"><span data-stu-id="29747-144">String</span></span>||
|<span data-ttu-id="29747-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="29747-145">startDateTime</span></span>|<span data-ttu-id="29747-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29747-146">DateTimeOffset</span></span>||
|<span data-ttu-id="29747-147">userId</span><span class="sxs-lookup"><span data-stu-id="29747-147">userId</span></span>|<span data-ttu-id="29747-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29747-148">String</span></span>||

## <a name="response"></a><span data-ttu-id="29747-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="29747-149">Response</span></span>

<span data-ttu-id="29747-150">Se tiver êxito, este método retornará `204 No Content` um código de resposta</span><span class="sxs-lookup"><span data-stu-id="29747-150">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="29747-151">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="29747-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="29747-152">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="29747-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="29747-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29747-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29747-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29747-154">Request</span></span>
<span data-ttu-id="29747-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29747-155">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="29747-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="29747-156">Response</span></span>
<span data-ttu-id="29747-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29747-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
