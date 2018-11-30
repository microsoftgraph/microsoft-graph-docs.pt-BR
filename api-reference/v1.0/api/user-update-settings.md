---
title: Configurações de atualização
description: 'Atualize as propriedades do objeto de configurações. '
ms.openlocfilehash: b763f2ccafeac84b12ff2e23cb89036afab5dbc7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005141"
---
# <a name="update-settings"></a><span data-ttu-id="da179-103">Configurações de atualização</span><span class="sxs-lookup"><span data-stu-id="da179-103">Update settings</span></span>

<span data-ttu-id="da179-104">Atualize as propriedades do objeto de [configurações](../resources/user-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="da179-104">Update the properties of the [settings](../resources/user-settings.md) object.</span></span> <span data-ttu-id="da179-105">Os usuários na mesma organização podem ter configurações diferentes com base em suas preferências ou nas diretivas de organização.</span><span class="sxs-lookup"><span data-stu-id="da179-105">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="da179-106">Para obter as configurações atuais de usuário, consulte [configurações do usuário atual](user-get-settings.md).</span><span class="sxs-lookup"><span data-stu-id="da179-106">To get the user current settings, see [current user settings](user-get-settings.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="da179-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="da179-107">Permissions</span></span>

<span data-ttu-id="da179-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da179-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da179-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da179-110">Permission type</span></span>      | <span data-ttu-id="da179-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da179-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da179-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da179-112">Delegated (work or school account)</span></span> | <span data-ttu-id="da179-113">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da179-113">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="da179-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da179-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da179-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da179-115">Not supported.</span></span>    |
|<span data-ttu-id="da179-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da179-116">Application</span></span> | <span data-ttu-id="da179-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da179-117">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da179-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da179-118">HTTP request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
```

<span data-ttu-id="da179-119">Solicitar com uma id de usuário' ' ou 'userPrincipalName' só está acessível pelo usuário ou por um usuário com as permissões User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="da179-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="da179-120">Para saber mais, consulte [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da179-120">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="da179-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da179-121">Request headers</span></span>

| <span data-ttu-id="da179-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da179-122">Header</span></span>       | <span data-ttu-id="da179-123">Valor</span><span class="sxs-lookup"><span data-stu-id="da179-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="da179-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="da179-124">Authorization</span></span>  | <span data-ttu-id="da179-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da179-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da179-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da179-127">Content-Type</span></span>  | <span data-ttu-id="da179-128">application/json</span><span class="sxs-lookup"><span data-stu-id="da179-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da179-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da179-129">Request body</span></span>

<span data-ttu-id="da179-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="da179-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="da179-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da179-133">Property</span></span>     | <span data-ttu-id="da179-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="da179-134">Type</span></span>   |<span data-ttu-id="da179-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="da179-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da179-136">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="da179-136">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="da179-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="da179-137">Boolean</span></span>|<span data-ttu-id="da179-138">Definido como verdadeiro desabilitar o acesso de representante a [tendência](/graph/api/resources/insights-trending?view=graph-rest-beta) API e para desabilitar o acesso a documentos do Office me aprofundar para o usuário.</span><span class="sxs-lookup"><span data-stu-id="da179-138">Set to true do disable delegate access to the [Trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="da179-139">Configuração como true também afeta a relevância do conteúdo exibido no Office 365 - por exemplo, sites sugeridos na página inicial do SharePoint e o modo de descoberta no OneDrive for Business mostram resultados menos relevantes.</span><span class="sxs-lookup"><span data-stu-id="da179-139">Setting to true also affects the relevance of the content displayed in Office 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="da179-140">Essa configuração reflete o estado de controle no [Office me aprofundar](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="da179-140">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="da179-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da179-141">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="da179-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da179-142">Request</span></span>

<span data-ttu-id="da179-143">Aqui está um exemplo de solicitação sobre como um usuário da Delve recusar e desabilitar a sua contribuição sobre relevância de conteúdo para a organização inteira.</span><span class="sxs-lookup"><span data-stu-id="da179-143">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="da179-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="da179-144">Response</span></span>

<span data-ttu-id="da179-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da179-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a><span data-ttu-id="da179-148">Solicitação em lote</span><span class="sxs-lookup"><span data-stu-id="da179-148">Batch request</span></span>

<span data-ttu-id="da179-149">Também é possível sair vários usuários do Delve e desabilitar pela sua contribuição sobre relevância de conteúdo para toda a organização por meio de uma solicitação de lote.</span><span class="sxs-lookup"><span data-stu-id="da179-149">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="da179-150">Para saber mais, consulte [JSON processamento em lotes](https://developer.microsoft.com/graph/docs/concepts/json_batching).</span><span class="sxs-lookup"><span data-stu-id="da179-150">To learn more, see [JSON batching](https://developer.microsoft.com/graph/docs/concepts/json_batching).</span></span>

<span data-ttu-id="da179-151">**Importante**: somente membros do grupo de funções de [Gerenciamento da organização](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) podem atualizar vários usuários.</span><span class="sxs-lookup"><span data-stu-id="da179-151">**Important**: Only members of the [Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 



