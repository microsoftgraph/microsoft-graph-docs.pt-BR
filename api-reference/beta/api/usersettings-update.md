---
title: Atualizar configurações
description: 'Atualize as propriedades do objeto de configurações. '
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1638c5716256988dc5bc36999ab3bebf7f068ee2
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896459"
---
# <a name="update-settings"></a><span data-ttu-id="76364-103">Atualizar configurações</span><span class="sxs-lookup"><span data-stu-id="76364-103">Update settings</span></span>

<span data-ttu-id="76364-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76364-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76364-105">Atualize as propriedades do objeto [UserSettings](../resources/usersettings.md) .</span><span class="sxs-lookup"><span data-stu-id="76364-105">Update the properties of the [userSettings](../resources/usersettings.md) object.</span></span> <span data-ttu-id="76364-106">Os usuários na mesma organização podem ter configurações diferentes com base em suas preferências ou nas políticas da organização.</span><span class="sxs-lookup"><span data-stu-id="76364-106">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="76364-107">Para obter as configurações atuais do usuário, confira [configurações atuais do usuário](usersettings-get.md).</span><span class="sxs-lookup"><span data-stu-id="76364-107">To get the user current settings, see [current user settings](usersettings-get.md).</span></span> 


### <a name="batch-request"></a><span data-ttu-id="76364-108">Solicitação em lote</span><span class="sxs-lookup"><span data-stu-id="76364-108">Batch request</span></span>

<span data-ttu-id="76364-109">Também é possível recusar vários usuários do Delve e desabilitar sua contribuição na relevância do conteúdo para toda a organização por meio de uma solicitação em lote.</span><span class="sxs-lookup"><span data-stu-id="76364-109">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="76364-110">Para saber mais, confira [Batching JSON](/graph/json-batching).</span><span class="sxs-lookup"><span data-stu-id="76364-110">To learn more, see [JSON batching](/graph/json-batching).</span></span>

><span data-ttu-id="76364-111">**Importante**: somente os membros do grupo de função [Gerenciamento da organização](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) podem atualizar vários usuários.</span><span class="sxs-lookup"><span data-stu-id="76364-111">**Important**: Only members of the [organization management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 



## <a name="permissions"></a><span data-ttu-id="76364-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="76364-112">Permissions</span></span>

<span data-ttu-id="76364-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76364-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76364-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76364-115">Permission type</span></span>      | <span data-ttu-id="76364-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76364-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76364-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76364-117">Delegated (work or school account)</span></span> | <span data-ttu-id="76364-118">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="76364-118">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="76364-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76364-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76364-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76364-120">Not supported.</span></span>    |
|<span data-ttu-id="76364-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76364-121">Application</span></span> | <span data-ttu-id="76364-122">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76364-122">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76364-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76364-123">HTTP request</span></span>

```http
PATCH /me/settings
```

<span data-ttu-id="76364-124">Solicitação com uma "id de usuário" ou "userPrincipalName" ficará acessível somente para o usuário ou um usuário com permissões User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="76364-124">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="76364-125">Para saber mais, confira [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76364-125">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH /users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="76364-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76364-126">Request headers</span></span>

| <span data-ttu-id="76364-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76364-127">Header</span></span>       | <span data-ttu-id="76364-128">Valor</span><span class="sxs-lookup"><span data-stu-id="76364-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="76364-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="76364-129">Authorization</span></span>  | <span data-ttu-id="76364-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76364-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="76364-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76364-132">Content-Type</span></span>  | <span data-ttu-id="76364-133">application/json</span><span class="sxs-lookup"><span data-stu-id="76364-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="76364-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76364-134">Request body</span></span>

<span data-ttu-id="76364-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="76364-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="76364-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76364-138">Property</span></span>     | <span data-ttu-id="76364-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="76364-139">Type</span></span>   |<span data-ttu-id="76364-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="76364-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76364-141">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="76364-141">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="76364-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="76364-142">Boolean</span></span>|<span data-ttu-id="76364-143">Defina como true para desabilitar o acesso de representante à API de [tendências](../resources/insights-trending.md) e desabilitar o acesso aos documentos no Office Delve para o usuário.</span><span class="sxs-lookup"><span data-stu-id="76364-143">Set to true do disable delegate access to the [Trending](../resources/insights-trending.md) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="76364-144">A configuração como true também afeta a relevância do conteúdo exibido no Microsoft 365-por exemplo, sites sugeridos na página inicial do SharePoint e o modo de exibição de descoberta no OneDrive for Business mostrar resultados menos relevantes.</span><span class="sxs-lookup"><span data-stu-id="76364-144">Setting to true also affects the relevance of the content displayed in Microsoft 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="76364-145">Essa configuração reflete o estado de controle no [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="76364-145">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="76364-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76364-146">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="76364-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76364-147">Request</span></span>

<span data-ttu-id="76364-148">Veja a seguir um exemplo de solicitação de como recusar um usuário de aprofundar e desabilitar sua contribuição na relevância do conteúdo para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="76364-148">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="76364-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="76364-149">Response</span></span>

<span data-ttu-id="76364-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76364-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

