---
title: Atualizar privilegedRoleSettings
description: Atualize as configurações de função para a configuração de função determinada. Um objeto privilegedRoleSettings será retornado.
localization_priority: Normal
ms.openlocfilehash: ce04a6e8c61c59f576d3a5e36592ba8ab4373de3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337243"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="ba01b-104">Atualizar privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="ba01b-104">Update privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba01b-105">Atualize as configurações de função para a configuração de função determinada.</span><span class="sxs-lookup"><span data-stu-id="ba01b-105">Update the role settings for the given role setting.</span></span> <span data-ttu-id="ba01b-106">Um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) será retornado.</span><span class="sxs-lookup"><span data-stu-id="ba01b-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="ba01b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba01b-107">Permissions</span></span>

<span data-ttu-id="ba01b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba01b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="ba01b-110">**Observação:** O solicitante deve ter uma das seguintes funções: administrador de função privilegiada, administrador global, administrador de segurança ou leitor de segurança.</span><span class="sxs-lookup"><span data-stu-id="ba01b-110">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="ba01b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba01b-111">Permission type</span></span>      | <span data-ttu-id="ba01b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba01b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba01b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba01b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ba01b-114">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="ba01b-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ba01b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba01b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba01b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba01b-116">Not supported.</span></span>    |
|<span data-ttu-id="ba01b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba01b-117">Application</span></span> | <span data-ttu-id="ba01b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba01b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba01b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba01b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="ba01b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba01b-120">Request headers</span></span>
| <span data-ttu-id="ba01b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ba01b-121">Name</span></span>      |<span data-ttu-id="ba01b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba01b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba01b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba01b-123">Authorization</span></span>  | <span data-ttu-id="ba01b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba01b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba01b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba01b-126">Request body</span></span>
<span data-ttu-id="ba01b-127">No corpo da solicitação, forneça uma representação JSON de um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="ba01b-127">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="ba01b-128">A tabela a seguir lista as propriedades que você pode fornecer ao atualizar uma configuração de função.</span><span class="sxs-lookup"><span data-stu-id="ba01b-128">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="ba01b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba01b-129">Property</span></span>|<span data-ttu-id="ba01b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba01b-130">Type</span></span>|<span data-ttu-id="ba01b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba01b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba01b-132">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="ba01b-132">elevationDuration</span></span>|<span data-ttu-id="ba01b-133">duration</span><span class="sxs-lookup"><span data-stu-id="ba01b-133">duration</span></span>|<span data-ttu-id="ba01b-134">A duração quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="ba01b-134">The duration when the role is activated.</span></span> <span data-ttu-id="ba01b-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba01b-135">Required.</span></span>|
|<span data-ttu-id="ba01b-136">id</span><span class="sxs-lookup"><span data-stu-id="ba01b-136">id</span></span>|<span data-ttu-id="ba01b-137">string</span><span class="sxs-lookup"><span data-stu-id="ba01b-137">string</span></span>|<span data-ttu-id="ba01b-138">O identificador exclusivo das configurações de função.</span><span class="sxs-lookup"><span data-stu-id="ba01b-138">The unique identifier for the role settings.</span></span> <span data-ttu-id="ba01b-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ba01b-139">Read-only.</span></span> <span data-ttu-id="ba01b-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba01b-140">Required.</span></span>|
|<span data-ttu-id="ba01b-141">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="ba01b-141">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="ba01b-142">booliano</span><span class="sxs-lookup"><span data-stu-id="ba01b-142">boolean</span></span>|<span data-ttu-id="ba01b-143">**true** se mfaOnElevation é configurável.</span><span class="sxs-lookup"><span data-stu-id="ba01b-143">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="ba01b-144">**false** se mfaOnElevation não é configurável.</span><span class="sxs-lookup"><span data-stu-id="ba01b-144">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="ba01b-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba01b-145">Required.</span></span>|
|<span data-ttu-id="ba01b-146">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="ba01b-146">lastGlobalAdmin</span></span>|<span data-ttu-id="ba01b-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba01b-147">Boolean</span></span>|<span data-ttu-id="ba01b-148">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="ba01b-148">For internal use only.</span></span>|
|<span data-ttu-id="ba01b-149">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="ba01b-149">maxElavationDuration</span></span>|<span data-ttu-id="ba01b-150">duration</span><span class="sxs-lookup"><span data-stu-id="ba01b-150">duration</span></span>|<span data-ttu-id="ba01b-151">Duração máxima da função ativada.</span><span class="sxs-lookup"><span data-stu-id="ba01b-151">Maximum duration for the activated role.</span></span> <span data-ttu-id="ba01b-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba01b-152">Required.</span></span>|
|<span data-ttu-id="ba01b-153">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="ba01b-153">mfaOnElevation</span></span>|<span data-ttu-id="ba01b-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba01b-154">Boolean</span></span>|<span data-ttu-id="ba01b-155">**true** se a MFA é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="ba01b-155">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="ba01b-156">**false** se a MFA não é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="ba01b-156">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="ba01b-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba01b-157">Required.</span></span>|
|<span data-ttu-id="ba01b-158">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="ba01b-158">minElevationDuration</span></span>|<span data-ttu-id="ba01b-159">duration</span><span class="sxs-lookup"><span data-stu-id="ba01b-159">duration</span></span>|<span data-ttu-id="ba01b-160">Duração mínima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="ba01b-160">Minimum duration for the activated role.</span></span> <span data-ttu-id="ba01b-161">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba01b-161">Required.</span></span>|
|<span data-ttu-id="ba01b-162">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="ba01b-162">notificationToUserOnElevation</span></span>|<span data-ttu-id="ba01b-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba01b-163">Boolean</span></span>|<span data-ttu-id="ba01b-164">**true** se enviar notificação para o usuário final quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="ba01b-164">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="ba01b-165">**false** se não enviar notificações quando a função for ativada.</span><span class="sxs-lookup"><span data-stu-id="ba01b-165">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="ba01b-166">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba01b-166">Required.</span></span>|
|<span data-ttu-id="ba01b-167">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="ba01b-167">ticketingInfoOnElevation</span></span>|<span data-ttu-id="ba01b-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba01b-168">Boolean</span></span>|<span data-ttu-id="ba01b-169">**true** se as informações de tíquete são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="ba01b-169">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="ba01b-170">**false** se as informações de tíquete não são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="ba01b-170">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="ba01b-171">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba01b-171">Required.</span></span>|
|<span data-ttu-id="ba01b-172">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="ba01b-172">approvalOnElevation</span></span>|<span data-ttu-id="ba01b-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba01b-173">Boolean</span></span>|<span data-ttu-id="ba01b-174">**true** se a aprovação é necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="ba01b-174">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="ba01b-175">**false** se a aprovação não é necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="ba01b-175">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="ba01b-176">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba01b-176">Required.</span></span>|
|<span data-ttu-id="ba01b-177">approverIds</span><span class="sxs-lookup"><span data-stu-id="ba01b-177">approverIds</span></span>|<span data-ttu-id="ba01b-178">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba01b-178">string collection</span></span>|<span data-ttu-id="ba01b-179">Lista de IDs de aprovação, se a aprovação for necessária para ativação.</span><span class="sxs-lookup"><span data-stu-id="ba01b-179">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="ba01b-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba01b-180">Response</span></span>

<span data-ttu-id="ba01b-181">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ba01b-181">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="ba01b-182">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="ba01b-182">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ba01b-183">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="ba01b-183">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="ba01b-184">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba01b-184">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba01b-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba01b-185">Request</span></span>
<span data-ttu-id="ba01b-186">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba01b-186">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ba01b-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba01b-187">Response</span></span>
<span data-ttu-id="ba01b-188">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba01b-188">Here is an example of the response.</span></span>
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
  "suppressions": []
}
-->
