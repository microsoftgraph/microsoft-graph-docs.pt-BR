---
title: Atualizar configurações
description: 'Atualize as propriedades do objeto de configurações. '
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: c22bc60ab37d5eb015896dc6832b0a72390d64a8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054284"
---
# <a name="update-settings"></a><span data-ttu-id="e4143-103">Atualizar configurações</span><span class="sxs-lookup"><span data-stu-id="e4143-103">Update settings</span></span>

<span data-ttu-id="e4143-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4143-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4143-105">Atualize as propriedades do [objeto userSettings.](../resources/usersettings.md)</span><span class="sxs-lookup"><span data-stu-id="e4143-105">Update the properties of the [userSettings](../resources/usersettings.md) object.</span></span> <span data-ttu-id="e4143-106">Os usuários na mesma organização podem ter configurações diferentes com base em suas preferências ou nas políticas da organização.</span><span class="sxs-lookup"><span data-stu-id="e4143-106">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="e4143-107">Para obter as configurações atuais do usuário, consulte [configurações atuais do usuário](usersettings-get.md).</span><span class="sxs-lookup"><span data-stu-id="e4143-107">To get the user current settings, see [current user settings](usersettings-get.md).</span></span> 

### <a name="batch-request"></a><span data-ttu-id="e4143-108">Solicitação em lote</span><span class="sxs-lookup"><span data-stu-id="e4143-108">Batch request</span></span>

<span data-ttu-id="e4143-109">Também é possível desativar vários usuários do Delve e desabilitar sua contribuição sobre a relevância do conteúdo para toda a organização por meio de uma solicitação em lotes.</span><span class="sxs-lookup"><span data-stu-id="e4143-109">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="e4143-110">Para saber mais, consulte [JSON batching](/graph/json-batching).</span><span class="sxs-lookup"><span data-stu-id="e4143-110">To learn more, see [JSON batching](/graph/json-batching).</span></span>

><span data-ttu-id="e4143-111">**Importante:** somente membros do grupo de função [de gerenciamento](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) da organização podem atualizar vários usuários.</span><span class="sxs-lookup"><span data-stu-id="e4143-111">**Important**: Only members of the [organization management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 



## <a name="permissions"></a><span data-ttu-id="e4143-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4143-112">Permissions</span></span>

<span data-ttu-id="e4143-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4143-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4143-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4143-115">Permission type</span></span>      | <span data-ttu-id="e4143-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4143-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4143-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4143-117">Delegated (work or school account)</span></span> | <span data-ttu-id="e4143-118">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4143-118">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="e4143-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4143-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4143-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4143-120">Not supported.</span></span>    |
|<span data-ttu-id="e4143-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4143-121">Application</span></span> | <span data-ttu-id="e4143-122">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4143-122">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4143-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4143-123">HTTP request</span></span>

```http
PATCH /me/settings
```

<span data-ttu-id="e4143-124">Solicitação com uma "id de usuário" ou "userPrincipalName" ficará acessível somente para o usuário ou um usuário com permissões User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="e4143-124">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="e4143-125">Para saber mais, confira [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4143-125">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH /users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="e4143-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4143-126">Request headers</span></span>

| <span data-ttu-id="e4143-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4143-127">Header</span></span>       | <span data-ttu-id="e4143-128">Valor</span><span class="sxs-lookup"><span data-stu-id="e4143-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e4143-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4143-129">Authorization</span></span>  | <span data-ttu-id="e4143-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4143-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e4143-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4143-132">Content-Type</span></span>  | <span data-ttu-id="e4143-133">application/json</span><span class="sxs-lookup"><span data-stu-id="e4143-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4143-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4143-134">Request body</span></span>

<span data-ttu-id="e4143-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e4143-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e4143-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4143-138">Property</span></span>     | <span data-ttu-id="e4143-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4143-139">Type</span></span>   |<span data-ttu-id="e4143-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4143-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4143-141">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="e4143-141">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="e4143-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="e4143-142">Boolean</span></span>|<span data-ttu-id="e4143-143">Definir como true desabilite o acesso de representante à API [de](/graph/api/resources/insights-trending?view=graph-rest-1.0) Tendência e desabilite o acesso aos documentos Office Delve para o usuário.</span><span class="sxs-lookup"><span data-stu-id="e4143-143">Set to true do disable delegate access to the [Trending](/graph/api/resources/insights-trending?view=graph-rest-1.0) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="e4143-144">A configuração como true também afeta a relevância do conteúdo exibido no Microsoft 365 - por exemplo, sites sugeridos no SharePoint Home e o exibição Descobrir no OneDrive for Business mostram resultados menos relevantes.</span><span class="sxs-lookup"><span data-stu-id="e4143-144">Setting to true also affects the relevance of the content displayed in Microsoft 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="e4143-145">Essa configuração reflete o estado de controle [em Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="e4143-145">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="e4143-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4143-146">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="e4143-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4143-147">Request</span></span>

<span data-ttu-id="e4143-148">Aqui está um exemplo de solicitação sobre como desativar um usuário do Delve e desabilitar sua contribuição sobre a relevância do conteúdo para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="e4143-148">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="e4143-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4143-149">Response</span></span>

<span data-ttu-id="e4143-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4143-150">Here is an example of the response.</span></span> <span data-ttu-id="e4143-151">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e4143-151">Note: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```