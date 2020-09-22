---
title: Tipo de recurso appRoleAssignment
description: Utilizado para registro quando um usuário, grupo ou entidade de serviço é atribuído a uma função de aplicativo na entidade de serviço de um aplicativo. Você pode criar, ler e excluir as atribuições de função.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: bc1649872955ee172ffa94c8c7316c82f49d0b8a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003336"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="ec4c1-104">Tipo de recurso appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ec4c1-104">appRoleAssignment resource type</span></span>

<span data-ttu-id="ec4c1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec4c1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec4c1-106">Utilizado para registro quando um usuário, grupo ou entidade de serviço recebe uma função de aplicativo para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-106">Used to record when a user, group, or service principal is assigned an app role for an app.</span></span>

<span data-ttu-id="ec4c1-107">Uma atribuição de função de aplicativo é uma relação entre a entidade de segurança atribuída (um usuário, um grupo ou uma entidade de serviço), um aplicativo de recursos (a entidade de serviço do aplicativo) e uma função de aplicativo definida no aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-107">An app role assignment is a relationship between the assigned principal (a user, a group, or a service principal), a resource application (the app's service principal) and an app role defined on the resource application.</span></span>

<span data-ttu-id="ec4c1-108">Quando a [função de aplicativo](approle.md) que foi atribuída a uma entidade tem uma propriedade de **valor** não vazio, isso será incluído nas **funções** de declaração de tokens em que o assunto é a entidade de segurança atribuída (por exemplo, respostas SAML, tokens de identificação, tokens de acesso identificando um usuário conectado ou um token de acesso identificando uma entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="ec4c1-108">When the [app role](approle.md) which has been assigned to a principal has a non-empty **value** property, this will be included in the **roles** claim of tokens where the subject is the  assigned principal (e.g. SAML responses, ID tokens, access tokens identifying a signed-in user, or an access token identifying a service principal).</span></span> <span data-ttu-id="ec4c1-109">Os aplicativos e as APIs usam essas declarações como parte da lógica de autorização.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-109">Applications and APIs use these claims as part of their authorization logic.</span></span>

<span data-ttu-id="ec4c1-110">É possível atribuir uma função de aplicativo diretamente a um usuário.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-110">A user can be assigned an app role directly.</span></span> <span data-ttu-id="ec4c1-111">Se uma função de aplicativo for atribuída a um grupo, os membros diretos do grupo também serão considerados atribuídos à função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-111">If an app role is assigned to a group, direct members of the group are also considered to have been assigned the app role.</span></span> <span data-ttu-id="ec4c1-112">Quando um usuário recebe uma função de aplicativo para um aplicativo, o bloco do aplicativo é exibido no portal [MyApps](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access) e no[inicializador de aplicativos do Microsoft 365](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a).</span><span class="sxs-lookup"><span data-stu-id="ec4c1-112">When a user is assigned an app role for an application, a tile for that application is displayed in the user's [MyApps portal](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access) and [Microsoft 365 app launcher](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a).</span></span>

<span data-ttu-id="ec4c1-113">Uma atribuição de função de aplicativo onde a entidade de segurança atribuída é uma entidade de serviço é uma permissão [somente para aplicativo](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="ec4c1-113">An app role assignment where the assigned principal is a service principal is an [app-only permission](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types) grant.</span></span> <span data-ttu-id="ec4c1-114">Quando um usuário ou administrador consentir a uma permissão somente para aplicativo, será criada uma atribuição de função de aplicativo onde a entidade de segurança atribuída é a entidade de serviço do aplicativo cliente e o recurso é a entidade de serviço da API de destino.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-114">When a user or admin consents to an app-only permission, an app role assignment is created where the assigned principal is the service principal for the client application, and the resource is the target API's service principal.</span></span>

## <a name="properties"></a><span data-ttu-id="ec4c1-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec4c1-115">Properties</span></span>

| <span data-ttu-id="ec4c1-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec4c1-116">Property</span></span> | <span data-ttu-id="ec4c1-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec4c1-117">Type</span></span> | <span data-ttu-id="ec4c1-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec4c1-118">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="ec4c1-119">id</span><span class="sxs-lookup"><span data-stu-id="ec4c1-119">id</span></span> | <span data-ttu-id="ec4c1-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec4c1-120">String</span></span> | <span data-ttu-id="ec4c1-121">Um identificador exclusivo para a chave **appRoleAssignment**.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-121">A unique identifier for the **appRoleAssignment** Key.</span></span> <span data-ttu-id="ec4c1-122">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-122">Not nullable.</span></span> <span data-ttu-id="ec4c1-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-123">Read-only.</span></span> |
| <span data-ttu-id="ec4c1-124">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="ec4c1-124">creationTimestamp</span></span> | <span data-ttu-id="ec4c1-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec4c1-125">DateTimeOffset</span></span> | <span data-ttu-id="ec4c1-126">A hora em que a atribuição de função do aplicativo foi criada. O tipo timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-126">The time when the app role assignment was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ec4c1-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ec4c1-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-128">Read-only.</span></span> <span data-ttu-id="ec4c1-129">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-129">Does not support `$filter`.</span></span> |
| <span data-ttu-id="ec4c1-130">principalId</span><span class="sxs-lookup"><span data-stu-id="ec4c1-130">principalId</span></span> | <span data-ttu-id="ec4c1-131">Guid</span><span class="sxs-lookup"><span data-stu-id="ec4c1-131">Guid</span></span> | <span data-ttu-id="ec4c1-132">O identificador exclusivo (**id**) para o [usuário](user.md), [grupo](group.md) ou da [entidade](serviceprincipal.md) a qual o acesso está sendo concedido.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-132">The unique identifier (**id**) for the [user](user.md), [group](group.md) or [service principal](serviceprincipal.md) being granted the app role.</span></span> <span data-ttu-id="ec4c1-133">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-133">Required on create.</span></span> <span data-ttu-id="ec4c1-134">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-134">Does not support `$filter`.</span></span> |
| <span data-ttu-id="ec4c1-135">principalType</span><span class="sxs-lookup"><span data-stu-id="ec4c1-135">principalType</span></span> | <span data-ttu-id="ec4c1-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec4c1-136">String</span></span> | <span data-ttu-id="ec4c1-137">O tipo da entidade de segurança atribuída.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-137">The type of the assigned principal.</span></span> <span data-ttu-id="ec4c1-138">Pode ser “User”, “Group” ou “ServicePrincipal”.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-138">This can either be "User", "Group" or "ServicePrincipal".</span></span> <span data-ttu-id="ec4c1-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-139">Read-only.</span></span> <span data-ttu-id="ec4c1-140">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-140">Does not support `$filter`.</span></span> |
| <span data-ttu-id="ec4c1-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="ec4c1-141">principalDisplayName</span></span> | <span data-ttu-id="ec4c1-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec4c1-142">String</span></span> |<span data-ttu-id="ec4c1-143">O nome de exibição do usuário, grupo ou entidade de serviço que recebeu a atribuição de função do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-143">The display name of the user, group, or service principal that was granted the app role assignment.</span></span> <span data-ttu-id="ec4c1-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-144">Read-only.</span></span> <span data-ttu-id="ec4c1-145">Suporte para `$filter` (`eq` e `startswith`).</span><span class="sxs-lookup"><span data-stu-id="ec4c1-145">Supports `$filter` (`eq` and `startswith`).</span></span> |
| <span data-ttu-id="ec4c1-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="ec4c1-146">resourceId</span></span> | <span data-ttu-id="ec4c1-147">Guid</span><span class="sxs-lookup"><span data-stu-id="ec4c1-147">Guid</span></span> |<span data-ttu-id="ec4c1-148">Identificador exclusivo (**id**) para o recurso [(entidade de serviço)](serviceprincipal.md) para o qual a atribuição foi feita.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-148">The unique identifier (**id**) for the resource [service principal](serviceprincipal.md) for which the assignment is made.</span></span> <span data-ttu-id="ec4c1-149">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-149">Required on create.</span></span> <span data-ttu-id="ec4c1-150">Suporte para `$filter` (`eq` somente).</span><span class="sxs-lookup"><span data-stu-id="ec4c1-150">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="ec4c1-151">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ec4c1-151">resourceDisplayName</span></span> | <span data-ttu-id="ec4c1-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec4c1-152">String</span></span> | <span data-ttu-id="ec4c1-153">O nome de exibição da entidade de serviço da função do aplicativo para o qual a atribuição foi feita.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-153">The display name of the resource app's service principal to which the assignment is made.</span></span> <span data-ttu-id="ec4c1-154">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-154">Does not support `$filter`.</span></span> |
| <span data-ttu-id="ec4c1-155">appRoleId</span><span class="sxs-lookup"><span data-stu-id="ec4c1-155">appRoleId</span></span> | <span data-ttu-id="ec4c1-156">Guid</span><span class="sxs-lookup"><span data-stu-id="ec4c1-156">Guid</span></span> | <span data-ttu-id="ec4c1-157">O identificador (**id**) da [função do aplicativo](approle.md) que está atribuída à entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-157">The identifier (**id**) for the [app role](approle.md) which is assigned to the principal.</span></span> <span data-ttu-id="ec4c1-158">Essa função de aplicativo deve ser exposta na propriedade **appRoles** na entidade de serviço do aplicativo de recurso (**ResourceId**).</span><span class="sxs-lookup"><span data-stu-id="ec4c1-158">This app role must be exposed in the **appRoles** property on the resource application's service principal (**resourceId**).</span></span> <span data-ttu-id="ec4c1-159">Se o aplicativo de recurso não tiver declarado todas as funções do aplicativo, uma ID de função de aplicativo padrão de `00000000-0000-0000-0000-000000000000` poderá ser especificada para sinalizar que a entidade de segurança está atribuída ao aplicativo de recursos sem nenhuma função específica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-159">If the resource application has not declared any app roles, a default app role ID of `00000000-0000-0000-0000-000000000000` can be specified to signal that the principal is assigned to the resource app without any specific app roles.</span></span> <span data-ttu-id="ec4c1-160">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-160">Required on create.</span></span> <span data-ttu-id="ec4c1-161">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ec4c1-161">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ec4c1-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec4c1-162">JSON representation</span></span>

<span data-ttu-id="ec4c1-163">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ec4c1-163">Here is a JSON representation of the resource</span></span>

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

