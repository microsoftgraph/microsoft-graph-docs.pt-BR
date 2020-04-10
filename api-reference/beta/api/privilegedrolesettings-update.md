---
title: Atualizar privilegedRoleSettings
description: Atualize as configurações de função para a configuração de função determinada. Um objeto privilegedRoleSettings será retornado.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 8cb9900ce5565cc2da4507ede841dbfeacdcb95e
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218651"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="5fbbe-104">Atualizar privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="5fbbe-104">Update privilegedRoleSettings</span></span>

<span data-ttu-id="5fbbe-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fbbe-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fbbe-106">Atualize as configurações de função para a configuração de função determinada.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-106">Update the role settings for the given role setting.</span></span> <span data-ttu-id="5fbbe-107">Um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) será retornado.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-107">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="5fbbe-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5fbbe-108">Permissions</span></span>

<span data-ttu-id="5fbbe-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fbbe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="5fbbe-111">**Observação:** O solicitante deve ter a função de administrador de função privilegiada para atualizar as configurações de função.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-111">**Note:** The requester must have the Privileged Role Administrator role to update role settings.</span></span> 

|<span data-ttu-id="5fbbe-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fbbe-112">Permission type</span></span>      | <span data-ttu-id="5fbbe-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5fbbe-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fbbe-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fbbe-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5fbbe-115">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="5fbbe-115">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5fbbe-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fbbe-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fbbe-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-117">Not supported.</span></span>    |
|<span data-ttu-id="5fbbe-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5fbbe-118">Application</span></span> | <span data-ttu-id="5fbbe-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fbbe-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fbbe-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="5fbbe-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fbbe-121">Request headers</span></span>
| <span data-ttu-id="5fbbe-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5fbbe-122">Name</span></span>      |<span data-ttu-id="5fbbe-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fbbe-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5fbbe-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fbbe-124">Authorization</span></span>  | <span data-ttu-id="5fbbe-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5fbbe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fbbe-127">Request body</span></span>
<span data-ttu-id="5fbbe-128">No corpo da solicitação, forneça uma representação JSON de um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="5fbbe-128">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="5fbbe-129">A tabela a seguir lista as propriedades que você pode fornecer ao atualizar uma configuração de função.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-129">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="5fbbe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fbbe-130">Property</span></span>|<span data-ttu-id="5fbbe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fbbe-131">Type</span></span>|<span data-ttu-id="5fbbe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fbbe-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fbbe-133">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="5fbbe-133">elevationDuration</span></span>|<span data-ttu-id="5fbbe-134">duration</span><span class="sxs-lookup"><span data-stu-id="5fbbe-134">duration</span></span>|<span data-ttu-id="5fbbe-135">A duração quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-135">The duration when the role is activated.</span></span> <span data-ttu-id="5fbbe-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-136">Required.</span></span>|
|<span data-ttu-id="5fbbe-137">id</span><span class="sxs-lookup"><span data-stu-id="5fbbe-137">id</span></span>|<span data-ttu-id="5fbbe-138">string</span><span class="sxs-lookup"><span data-stu-id="5fbbe-138">string</span></span>|<span data-ttu-id="5fbbe-139">O identificador exclusivo das configurações de função.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-139">The unique identifier for the role settings.</span></span> <span data-ttu-id="5fbbe-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-140">Read-only.</span></span> <span data-ttu-id="5fbbe-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-141">Required.</span></span>|
|<span data-ttu-id="5fbbe-142">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="5fbbe-142">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="5fbbe-143">booliano</span><span class="sxs-lookup"><span data-stu-id="5fbbe-143">boolean</span></span>|<span data-ttu-id="5fbbe-144">**true** se mfaOnElevation é configurável.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-144">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="5fbbe-145">**false** se mfaOnElevation não é configurável.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-145">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="5fbbe-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-146">Required.</span></span>|
|<span data-ttu-id="5fbbe-147">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="5fbbe-147">lastGlobalAdmin</span></span>|<span data-ttu-id="5fbbe-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbbe-148">Boolean</span></span>|<span data-ttu-id="5fbbe-149">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-149">For internal use only.</span></span>|
|<span data-ttu-id="5fbbe-150">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="5fbbe-150">maxElavationDuration</span></span>|<span data-ttu-id="5fbbe-151">duration</span><span class="sxs-lookup"><span data-stu-id="5fbbe-151">duration</span></span>|<span data-ttu-id="5fbbe-152">Duração máxima da função ativada.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-152">Maximum duration for the activated role.</span></span> <span data-ttu-id="5fbbe-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-153">Required.</span></span>|
|<span data-ttu-id="5fbbe-154">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="5fbbe-154">mfaOnElevation</span></span>|<span data-ttu-id="5fbbe-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbbe-155">Boolean</span></span>|<span data-ttu-id="5fbbe-156">**true** se a MFA é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-156">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="5fbbe-157">**false** se a MFA não é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-157">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="5fbbe-158">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-158">Required.</span></span>|
|<span data-ttu-id="5fbbe-159">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="5fbbe-159">minElevationDuration</span></span>|<span data-ttu-id="5fbbe-160">duration</span><span class="sxs-lookup"><span data-stu-id="5fbbe-160">duration</span></span>|<span data-ttu-id="5fbbe-161">Duração mínima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-161">Minimum duration for the activated role.</span></span> <span data-ttu-id="5fbbe-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-162">Required.</span></span>|
|<span data-ttu-id="5fbbe-163">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="5fbbe-163">notificationToUserOnElevation</span></span>|<span data-ttu-id="5fbbe-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbbe-164">Boolean</span></span>|<span data-ttu-id="5fbbe-165">**true** se enviar notificação para o usuário final quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-165">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="5fbbe-166">**false** se não enviar notificações quando a função for ativada.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-166">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="5fbbe-167">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-167">Required.</span></span>|
|<span data-ttu-id="5fbbe-168">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="5fbbe-168">ticketingInfoOnElevation</span></span>|<span data-ttu-id="5fbbe-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbbe-169">Boolean</span></span>|<span data-ttu-id="5fbbe-170">**true** se as informações de tíquete são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-170">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="5fbbe-171">**false** se as informações de tíquete não são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-171">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="5fbbe-172">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-172">Required.</span></span>|
|<span data-ttu-id="5fbbe-173">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="5fbbe-173">approvalOnElevation</span></span>|<span data-ttu-id="5fbbe-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbbe-174">Boolean</span></span>|<span data-ttu-id="5fbbe-175">**true** se a aprovação é necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-175">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="5fbbe-176">**false** se a aprovação não é necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-176">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="5fbbe-177">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-177">Required.</span></span>|
|<span data-ttu-id="5fbbe-178">approverIds</span><span class="sxs-lookup"><span data-stu-id="5fbbe-178">approverIds</span></span>|<span data-ttu-id="5fbbe-179">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fbbe-179">string collection</span></span>|<span data-ttu-id="5fbbe-180">Lista de IDs de aprovação, se a aprovação for necessária para ativação.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-180">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="5fbbe-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fbbe-181">Response</span></span>

<span data-ttu-id="5fbbe-182">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-182">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="5fbbe-183">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-183">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="5fbbe-184">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-184">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="5fbbe-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5fbbe-185">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5fbbe-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fbbe-186">Request</span></span>
<span data-ttu-id="5fbbe-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-187">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5fbbe-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fbbe-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_privilegedrolesettings"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
Content-type: application/json

{
    "id": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "elevationDuration": "PT8H",
    "notificationToUserOnElevation": false,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": false,
    "maxElavationDuration": "PT0S",
    "minElevationDuration": "PT0S",
    "lastGlobalAdmin": false,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": false,
    "approverIds": ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
}
```
# <a name="c"></a>[<span data-ttu-id="5fbbe-189">C#</span><span class="sxs-lookup"><span data-stu-id="5fbbe-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5fbbe-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fbbe-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5fbbe-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fbbe-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5fbbe-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fbbe-192">Response</span></span>
<span data-ttu-id="5fbbe-193">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fbbe-193">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
