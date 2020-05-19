---
title: Tipo de recurso plannerAssignment
description: Usado para gravar quando um usuário, grupo ou entidade de serviço é atribuído a uma função de aplicativo na entidade de serviço de um aplicativo. Você pode criar, ler e excluir atribuições de função de aplicativo.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 38f8cca5740da2cbd9807cd2411065a6bebda49c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291003"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="f6121-104">Tipo de recurso plannerAssignment</span><span class="sxs-lookup"><span data-stu-id="f6121-104">appRoleAssignment resource type</span></span>

<span data-ttu-id="f6121-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6121-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6121-106">Usado para gravar quando um usuário, grupo ou entidade de serviço recebe uma função de aplicativo para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6121-106">Used to record when a user, group, or service principal is assigned an app role for an app.</span></span>

<span data-ttu-id="f6121-107">Uma atribuição de função de aplicativo é uma relação entre a entidade de segurança atribuída (um usuário, um grupo ou uma entidade de serviço), um aplicativo de recurso (a entidade de serviço do aplicativo) e uma função de aplicativo definida no aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="f6121-107">An app role assignment is a relationship between the assigned principal (a user, a group, or a service principal), a resource application (the app's service principal) and an app role defined on the resource application.</span></span>

<span data-ttu-id="f6121-108">Quando a [função de aplicativo](approle.md) que foi atribuída a uma entidade de segurança tem uma propriedade de **valor** não vazio, ela será incluída na declaração de **funções** de tokens em que o assunto é a entidade de segurança atribuída (por exemplo, respostas SAML, tokens de ID, tokens de acesso que identificam um usuário conectado ou um token de acesso que identifica uma entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="f6121-108">When the [app role](approle.md) which has been assigned to a principal has a non-empty **value** property, this will be included in the **roles** claim of tokens where the subject is the  assigned principal (e.g. SAML responses, ID tokens, access tokens identifying a signed-in user, or an access token identifying a service principal).</span></span> <span data-ttu-id="f6121-109">Aplicativos e APIs usam essas declarações como parte de sua lógica de autorização.</span><span class="sxs-lookup"><span data-stu-id="f6121-109">Applications and APIs use these claims as part of their authorization logic.</span></span>

<span data-ttu-id="f6121-110">Um usuário pode ser atribuído diretamente a uma função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6121-110">A user can be assigned an app role directly.</span></span> <span data-ttu-id="f6121-111">Se uma função de aplicativo for atribuída a um grupo, os membros diretos do grupo também serão considerados como a função de aplicativo atribuída.</span><span class="sxs-lookup"><span data-stu-id="f6121-111">If an app role is assigned to a group, direct members of the group are also considered to have been assigned the app role.</span></span> <span data-ttu-id="f6121-112">Quando um usuário recebe uma função de aplicativo para um aplicativo, um bloco para esse aplicativo é exibido no [portal myapps](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access) do usuário e no [inicializador de aplicativos do Office 365](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a).</span><span class="sxs-lookup"><span data-stu-id="f6121-112">When a user is assigned an app role for an application, a tile for that application is displayed in the user's [MyApps portal](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access) and [Office 365 app launcher](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a).</span></span>

<span data-ttu-id="f6121-113">Uma atribuição de função de aplicativo onde a entidade atribuída é uma entidade de serviço é uma concessão [de permissão somente de aplicativo](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types) .</span><span class="sxs-lookup"><span data-stu-id="f6121-113">An app role assignment where the assigned principal is a service principal is an [app-only permission](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types) grant.</span></span> <span data-ttu-id="f6121-114">Quando um usuário ou administrador se envia a uma permissão somente de aplicativo, uma atribuição de função de aplicativo é criada onde a entidade de segurança atribuída é a entidade de serviço para o aplicativo cliente e o recurso é a entidade de serviço da API de destino.</span><span class="sxs-lookup"><span data-stu-id="f6121-114">When a user or admin consents to an app-only permission, an app role assignment is created where the assigned principal is the service principal for the client application, and the resource is the target API's service principal.</span></span>

## <a name="properties"></a><span data-ttu-id="f6121-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6121-115">Properties</span></span>

| <span data-ttu-id="f6121-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6121-116">Property</span></span> | <span data-ttu-id="f6121-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6121-117">Type</span></span> | <span data-ttu-id="f6121-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6121-118">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="f6121-119">id</span><span class="sxs-lookup"><span data-stu-id="f6121-119">id</span></span> | <span data-ttu-id="f6121-120">String</span><span class="sxs-lookup"><span data-stu-id="f6121-120">String</span></span> | <span data-ttu-id="f6121-121">Um identificador exclusivo para a chave **appRoleAssignment** .</span><span class="sxs-lookup"><span data-stu-id="f6121-121">A unique identifier for the **appRoleAssignment** Key.</span></span> <span data-ttu-id="f6121-122">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="f6121-122">Not nullable.</span></span> <span data-ttu-id="f6121-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6121-123">Read-only.</span></span> |
| <span data-ttu-id="f6121-124">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="f6121-124">creationTimestamp</span></span> | <span data-ttu-id="f6121-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6121-125">DateTimeOffset</span></span> | <span data-ttu-id="f6121-126">A hora em que a atribuição de função de aplicativo foi criada. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f6121-126">The time when the app role assignment was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f6121-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f6121-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f6121-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6121-128">Read-only.</span></span> <span data-ttu-id="f6121-129">Não oferece suporte `$filter` .</span><span class="sxs-lookup"><span data-stu-id="f6121-129">Does not support `$filter`.</span></span> |
| <span data-ttu-id="f6121-130">principalId</span><span class="sxs-lookup"><span data-stu-id="f6121-130">principalId</span></span> | <span data-ttu-id="f6121-131">Guid</span><span class="sxs-lookup"><span data-stu-id="f6121-131">Guid</span></span> | <span data-ttu-id="f6121-132">O identificador exclusivo (**ID**) do [usuário](user.md), [grupo](group.md) ou [entidade de serviço](serviceprincipal.md) que recebeu a função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6121-132">The unique identifier (**id**) for the [user](user.md), [group](group.md) or [service principal](serviceprincipal.md) being granted the app role.</span></span> <span data-ttu-id="f6121-133">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="f6121-133">Required on create.</span></span> <span data-ttu-id="f6121-134">Não oferece suporte `$filter` .</span><span class="sxs-lookup"><span data-stu-id="f6121-134">Does not support `$filter`.</span></span> |
| <span data-ttu-id="f6121-135">principalType</span><span class="sxs-lookup"><span data-stu-id="f6121-135">principalType</span></span> | <span data-ttu-id="f6121-136">String</span><span class="sxs-lookup"><span data-stu-id="f6121-136">String</span></span> | <span data-ttu-id="f6121-137">O tipo da entidade de segurança atribuída.</span><span class="sxs-lookup"><span data-stu-id="f6121-137">The type of the assigned principal.</span></span> <span data-ttu-id="f6121-138">Pode ser “User”, “Group” ou “ServicePrincipal”.</span><span class="sxs-lookup"><span data-stu-id="f6121-138">This can either be "User", "Group" or "ServicePrincipal".</span></span> <span data-ttu-id="f6121-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6121-139">Read-only.</span></span> <span data-ttu-id="f6121-140">Não oferece suporte `$filter` .</span><span class="sxs-lookup"><span data-stu-id="f6121-140">Does not support `$filter`.</span></span> |
| <span data-ttu-id="f6121-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="f6121-141">principalDisplayName</span></span> | <span data-ttu-id="f6121-142">String</span><span class="sxs-lookup"><span data-stu-id="f6121-142">String</span></span> |<span data-ttu-id="f6121-143">O nome de exibição do usuário, grupo ou entidade de serviço que recebeu a atribuição da função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6121-143">The display name of the user, group, or service principal that was granted the app role assignment.</span></span> <span data-ttu-id="f6121-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6121-144">Read-only.</span></span> <span data-ttu-id="f6121-145">Suporta `$filter` ( `eq` e `startswith` ).</span><span class="sxs-lookup"><span data-stu-id="f6121-145">Supports `$filter` (`eq` and `startswith`).</span></span> |
| <span data-ttu-id="f6121-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="f6121-146">resourceId</span></span> | <span data-ttu-id="f6121-147">Guid</span><span class="sxs-lookup"><span data-stu-id="f6121-147">Guid</span></span> |<span data-ttu-id="f6121-148">O identificador exclusivo (**ID**) da entidade de [serviço](serviceprincipal.md) de recurso para a qual a atribuição foi feita.</span><span class="sxs-lookup"><span data-stu-id="f6121-148">The unique identifier (**id**) for the resource [service principal](serviceprincipal.md) for which the assignment is made.</span></span> <span data-ttu-id="f6121-149">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="f6121-149">Required on create.</span></span> <span data-ttu-id="f6121-150">Suporta `$filter` ( `eq` somente).</span><span class="sxs-lookup"><span data-stu-id="f6121-150">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="f6121-151">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f6121-151">resourceDisplayName</span></span> | <span data-ttu-id="f6121-152">String</span><span class="sxs-lookup"><span data-stu-id="f6121-152">String</span></span> | <span data-ttu-id="f6121-153">O nome de exibição da entidade de serviço do aplicativo de recurso para a qual a atribuição foi feita.</span><span class="sxs-lookup"><span data-stu-id="f6121-153">The display name of the resource app's service principal to which the assignment is made.</span></span> <span data-ttu-id="f6121-154">Não oferece suporte `$filter` .</span><span class="sxs-lookup"><span data-stu-id="f6121-154">Does not support `$filter`.</span></span> |
| <span data-ttu-id="f6121-155">appRoleId</span><span class="sxs-lookup"><span data-stu-id="f6121-155">appRoleId</span></span> | <span data-ttu-id="f6121-156">Guid</span><span class="sxs-lookup"><span data-stu-id="f6121-156">Guid</span></span> | <span data-ttu-id="f6121-157">O identificador (**ID**) da [função de aplicativo](approle.md) que é atribuída à entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="f6121-157">The identifier (**id**) for the [app role](approle.md) which is assigned to the principal.</span></span> <span data-ttu-id="f6121-158">Essa função de aplicativo deve ser exposta na propriedade **appRoles** na entidade de serviço do aplicativo de recurso (**ResourceId**).</span><span class="sxs-lookup"><span data-stu-id="f6121-158">This app role must be exposed in the **appRoles** property on the resource application's service principal (**resourceId**).</span></span> <span data-ttu-id="f6121-159">Se o aplicativo de recursos não tiver declarado nenhuma função de aplicativo, uma ID de função de aplicativo padrão `00000000-0000-0000-0000-000000000000` pode ser especificada para sinalizar que a entidade de segurança é atribuída ao aplicativo de recursos sem nenhuma função de aplicativo específica.</span><span class="sxs-lookup"><span data-stu-id="f6121-159">If the resource application has not declared any app roles, a default app role ID of `00000000-0000-0000-0000-000000000000` can be specified to signal that the principal is assigned to the resource app without any specific app roles.</span></span> <span data-ttu-id="f6121-160">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="f6121-160">Required on create.</span></span> <span data-ttu-id="f6121-161">Não oferece suporte `$filter` .</span><span class="sxs-lookup"><span data-stu-id="f6121-161">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f6121-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6121-162">JSON representation</span></span>

<span data-ttu-id="f6121-163">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f6121-163">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
}-->

```json
{
  "id": "string",
  "creationTimestamp": "String (timestamp)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid",
  "appRoleId": "guid"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
