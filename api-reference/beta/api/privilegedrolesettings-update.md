---
title: Atualizar privilegedRoleSettings
description: Atualize as configurações de função para a configuração de determinada função. Um objeto privilegedRoleSettings será retornado.
localization_priority: Normal
ms.openlocfilehash: 7c117abfe774eae60e42dcbc5f748c10cacf5cd6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819310"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="f89fd-104">Atualizar privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="f89fd-104">Update privilegedRoleSettings</span></span>

> <span data-ttu-id="f89fd-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f89fd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f89fd-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f89fd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f89fd-107">Atualize as configurações de função para a configuração de determinada função.</span><span class="sxs-lookup"><span data-stu-id="f89fd-107">Update the role settings for the given role setting.</span></span> <span data-ttu-id="f89fd-108">Um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) será retornado.</span><span class="sxs-lookup"><span data-stu-id="f89fd-108">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="f89fd-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="f89fd-109">Permissions</span></span>

<span data-ttu-id="f89fd-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f89fd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="f89fd-112">**Observação:** O solicitante deve ter uma das seguintes funções: leitor de segurança, Administrador Global, administrador de segurança ou administrador com privilégios de função.</span><span class="sxs-lookup"><span data-stu-id="f89fd-112">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="f89fd-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f89fd-113">Permission type</span></span>      | <span data-ttu-id="f89fd-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f89fd-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f89fd-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f89fd-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f89fd-116">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f89fd-116">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f89fd-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f89fd-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f89fd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f89fd-118">Not supported.</span></span>    |
|<span data-ttu-id="f89fd-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f89fd-119">Application</span></span> | <span data-ttu-id="f89fd-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f89fd-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f89fd-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f89fd-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="f89fd-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f89fd-122">Request headers</span></span>
| <span data-ttu-id="f89fd-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f89fd-123">Name</span></span>      |<span data-ttu-id="f89fd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f89fd-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f89fd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f89fd-125">Authorization</span></span>  | <span data-ttu-id="f89fd-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f89fd-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f89fd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f89fd-128">Request body</span></span>
<span data-ttu-id="f89fd-129">No corpo da solicitação, fornece uma representação JSON de um objeto [privilegedRoleSettings](../resources/privilegedrolesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="f89fd-129">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="f89fd-130">A tabela a seguir lista as propriedades que você pode fornecer ao atualizar uma configuração de função.</span><span class="sxs-lookup"><span data-stu-id="f89fd-130">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="f89fd-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f89fd-131">Property</span></span>|<span data-ttu-id="f89fd-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f89fd-132">Type</span></span>|<span data-ttu-id="f89fd-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f89fd-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f89fd-134">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="f89fd-134">elevationDuration</span></span>|<span data-ttu-id="f89fd-135">duration</span><span class="sxs-lookup"><span data-stu-id="f89fd-135">duration</span></span>|<span data-ttu-id="f89fd-136">A duração quando a função for ativada.</span><span class="sxs-lookup"><span data-stu-id="f89fd-136">The duration when the role is activated.</span></span> <span data-ttu-id="f89fd-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f89fd-137">Required.</span></span>|
|<span data-ttu-id="f89fd-138">id</span><span class="sxs-lookup"><span data-stu-id="f89fd-138">id</span></span>|<span data-ttu-id="f89fd-139">string</span><span class="sxs-lookup"><span data-stu-id="f89fd-139">string</span></span>|<span data-ttu-id="f89fd-140">O identificador exclusivo para as configurações de função.</span><span class="sxs-lookup"><span data-stu-id="f89fd-140">The unique identifier for the role settings.</span></span> <span data-ttu-id="f89fd-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f89fd-141">Read-only.</span></span> <span data-ttu-id="f89fd-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f89fd-142">Required.</span></span>|
|<span data-ttu-id="f89fd-143">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="f89fd-143">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="f89fd-144">booliano</span><span class="sxs-lookup"><span data-stu-id="f89fd-144">boolean</span></span>|<span data-ttu-id="f89fd-145">**true** se mfaOnElevation é configurável.</span><span class="sxs-lookup"><span data-stu-id="f89fd-145">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="f89fd-146">**false** se mfaOnElevation não é configurável.</span><span class="sxs-lookup"><span data-stu-id="f89fd-146">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="f89fd-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f89fd-147">Required.</span></span>|
|<span data-ttu-id="f89fd-148">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="f89fd-148">lastGlobalAdmin</span></span>|<span data-ttu-id="f89fd-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="f89fd-149">Boolean</span></span>|<span data-ttu-id="f89fd-150">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="f89fd-150">For internal use only.</span></span>|
|<span data-ttu-id="f89fd-151">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="f89fd-151">maxElavationDuration</span></span>|<span data-ttu-id="f89fd-152">duration</span><span class="sxs-lookup"><span data-stu-id="f89fd-152">duration</span></span>|<span data-ttu-id="f89fd-153">Duração máxima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="f89fd-153">Maximum duration for the activated role.</span></span> <span data-ttu-id="f89fd-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f89fd-154">Required.</span></span>|
|<span data-ttu-id="f89fd-155">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="f89fd-155">mfaOnElevation</span></span>|<span data-ttu-id="f89fd-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="f89fd-156">Boolean</span></span>|<span data-ttu-id="f89fd-157">**true** se MFA é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="f89fd-157">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="f89fd-158">**false** se MFA não é necessário para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="f89fd-158">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="f89fd-159">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f89fd-159">Required.</span></span>|
|<span data-ttu-id="f89fd-160">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="f89fd-160">minElevationDuration</span></span>|<span data-ttu-id="f89fd-161">duration</span><span class="sxs-lookup"><span data-stu-id="f89fd-161">duration</span></span>|<span data-ttu-id="f89fd-162">Duração mínima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="f89fd-162">Minimum duration for the activated role.</span></span> <span data-ttu-id="f89fd-163">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f89fd-163">Required.</span></span>|
|<span data-ttu-id="f89fd-164">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="f89fd-164">notificationToUserOnElevation</span></span>|<span data-ttu-id="f89fd-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="f89fd-165">Boolean</span></span>|<span data-ttu-id="f89fd-166">**True** se enviar notificação ao usuário final quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="f89fd-166">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="f89fd-167">**False** se não enviar notificação quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="f89fd-167">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="f89fd-168">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f89fd-168">Required.</span></span>|
|<span data-ttu-id="f89fd-169">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="f89fd-169">ticketingInfoOnElevation</span></span>|<span data-ttu-id="f89fd-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="f89fd-170">Boolean</span></span>|<span data-ttu-id="f89fd-171">**true** se as informações de tickets são necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="f89fd-171">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="f89fd-172">**false** se as informações de tickets não são necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="f89fd-172">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="f89fd-173">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f89fd-173">Required.</span></span>|
|<span data-ttu-id="f89fd-174">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="f89fd-174">approvalOnElevation</span></span>|<span data-ttu-id="f89fd-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="f89fd-175">Boolean</span></span>|<span data-ttu-id="f89fd-176">**true** se a aprovação é necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="f89fd-176">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="f89fd-177">**false** se a aprovação não é necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="f89fd-177">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="f89fd-178">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f89fd-178">Required.</span></span>|
|<span data-ttu-id="f89fd-179">approverIds</span><span class="sxs-lookup"><span data-stu-id="f89fd-179">approverIds</span></span>|<span data-ttu-id="f89fd-180">array</span><span class="sxs-lookup"><span data-stu-id="f89fd-180">array</span></span>|<span data-ttu-id="f89fd-181">Lista de IDs de aprovação, se a aprovação é necessária para a ativação.</span><span class="sxs-lookup"><span data-stu-id="f89fd-181">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="f89fd-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="f89fd-182">Response</span></span>

<span data-ttu-id="f89fd-183">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f89fd-183">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="f89fd-184">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="f89fd-184">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="f89fd-185">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="f89fd-185">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="f89fd-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f89fd-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f89fd-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f89fd-187">Request</span></span>
<span data-ttu-id="f89fd-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f89fd-188">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="f89fd-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="f89fd-189">Response</span></span>
<span data-ttu-id="f89fd-190">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f89fd-190">Here is an example of the response.</span></span>

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
