---
title: Inscrições de lista
description: " Consulte os cenários abaixo para obter detalhes."
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 20aad712bc49f91bec58a67c0c66ef76bf4653e2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510978"
---
# <a name="list-subscriptions"></a><span data-ttu-id="10937-103">Inscrições de lista</span><span class="sxs-lookup"><span data-stu-id="10937-103">List subscriptions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10937-104">Recupere uma lista das inscrições de webhook.</span><span class="sxs-lookup"><span data-stu-id="10937-104">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="10937-105">O conteúdo da resposta depende do contexto no qual o aplicativo está chamando; Consulte os cenários abaixo para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="10937-105">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="10937-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="10937-106">Permissions</span></span>

<span data-ttu-id="10937-107">Essa API suporta os seguintes escopos de permissão; Para saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10937-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10937-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10937-108">Permission type</span></span>  | <span data-ttu-id="10937-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10937-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="10937-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10937-110">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="10937-111">Permissão necessária para [criar a inscrição](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="10937-111">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="10937-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10937-112">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="10937-113">Permissão necessária para [criar a inscrição](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="10937-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="10937-114">Application</span><span class="sxs-lookup"><span data-stu-id="10937-114">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="10937-115">Permissão necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="10937-115">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="10937-116">Resultados de resposta são baseados no contexto do aplicativo chamado.</span><span class="sxs-lookup"><span data-stu-id="10937-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="10937-117">Apresentamos a seguir um resumo dos cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="10937-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="10937-118">Cenários básicos</span><span class="sxs-lookup"><span data-stu-id="10937-118">Basic scenarios</span></span>

<span data-ttu-id="10937-119">Mais comumente, um aplicativo deseja recuperar as assinaturas que originalmente criado para o usuário conectado no momento, ou para todos os usuários no diretório (contas de trabalho/escola).</span><span class="sxs-lookup"><span data-stu-id="10937-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="10937-120">Esses cenários não exigem qualquer permissões especiais além do aplicativo originalmente usado para criar suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="10937-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="10937-121">Contexto do aplicativo chamado</span><span class="sxs-lookup"><span data-stu-id="10937-121">Context of the calling app</span></span> | <span data-ttu-id="10937-122">Resposta conterá</span><span class="sxs-lookup"><span data-stu-id="10937-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="10937-123">App está chamando em nome do usuário conectado (delegada permissão).</span><span class="sxs-lookup"><span data-stu-id="10937-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="10937-124">And</span><span class="sxs-lookup"><span data-stu-id="10937-124">-and-</span></span><br/><span data-ttu-id="10937-125">App tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="10937-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="10937-126">Observação: Isso se aplica ao pessoais contas da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="10937-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="10937-127">Inscrições criadas por **Este aplicativo** para o usuário entrou no apenas.</span><span class="sxs-lookup"><span data-stu-id="10937-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="10937-128">App está chamando em nome do próprio (permissão de aplicativo).</span><span class="sxs-lookup"><span data-stu-id="10937-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="10937-129">And</span><span class="sxs-lookup"><span data-stu-id="10937-129">-and-</span></span><br/><span data-ttu-id="10937-130">App tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="10937-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="10937-131">Observação: Isso se aplica a apenas contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="10937-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="10937-132">Inscrições criadas por **Este aplicativo** para si mesmo ou para qualquer usuário no diretório.</span><span class="sxs-lookup"><span data-stu-id="10937-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="10937-133">Cenários avançados</span><span class="sxs-lookup"><span data-stu-id="10937-133">Advanced scenarios</span></span>

<span data-ttu-id="10937-134">Em alguns casos, um aplicativo quer recuperar inscrições criadas por outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="10937-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="10937-135">Por exemplo, um usuário quiser ver todas as inscrições criadas por qualquer aplicativo em nome deles.</span><span class="sxs-lookup"><span data-stu-id="10937-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="10937-136">Ou então, um administrador talvez queira ver todas as inscrições de todos os aplicativos no seu diretório.</span><span class="sxs-lookup"><span data-stu-id="10937-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="10937-137">Para nesses cenários, uma permissão delegada Subscription.Read.All é necessária.</span><span class="sxs-lookup"><span data-stu-id="10937-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="10937-138">Contexto do aplicativo chamado</span><span class="sxs-lookup"><span data-stu-id="10937-138">Context of the calling app</span></span> | <span data-ttu-id="10937-139">Resposta conterá</span><span class="sxs-lookup"><span data-stu-id="10937-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="10937-140">App está chamando em nome do usuário conectado (delegada permissão).</span><span class="sxs-lookup"><span data-stu-id="10937-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="10937-141">*O usuário é um não seja o administrador*.</span><span class="sxs-lookup"><span data-stu-id="10937-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="10937-142">And</span><span class="sxs-lookup"><span data-stu-id="10937-142">-and-</span></span><br/><span data-ttu-id="10937-143">App tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="10937-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="10937-144">Observação: Isso se aplica ao pessoais contas da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="10937-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="10937-145">Inscrições criadas por **qualquer aplicativo** para o usuário entrou no apenas.</span><span class="sxs-lookup"><span data-stu-id="10937-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="10937-146">App está chamando em nome do usuário conectado (delegada permissão).</span><span class="sxs-lookup"><span data-stu-id="10937-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="10937-147">*O usuário é um administrador*.</span><span class="sxs-lookup"><span data-stu-id="10937-147">*The user is an admin*.</span></span><br/><span data-ttu-id="10937-148">And</span><span class="sxs-lookup"><span data-stu-id="10937-148">-and-</span></span><br/><span data-ttu-id="10937-149">App tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="10937-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="10937-150">Observação: Isso se aplica a apenas contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="10937-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="10937-151">Inscrições criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.</span><span class="sxs-lookup"><span data-stu-id="10937-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10937-152">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10937-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10937-153">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="10937-153">Optional query parameters</span></span>

<span data-ttu-id="10937-154">Este método não oferece suporte para os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="10937-154">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10937-155">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10937-155">Request headers</span></span>

| <span data-ttu-id="10937-156">Nome</span><span class="sxs-lookup"><span data-stu-id="10937-156">Name</span></span>       | <span data-ttu-id="10937-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="10937-157">Type</span></span> | <span data-ttu-id="10937-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="10937-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="10937-159">Autorização</span><span class="sxs-lookup"><span data-stu-id="10937-159">Authorization</span></span>  | <span data-ttu-id="10937-160">string</span><span class="sxs-lookup"><span data-stu-id="10937-160">string</span></span>  | <span data-ttu-id="10937-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10937-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10937-163">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10937-163">Request body</span></span>

<span data-ttu-id="10937-164">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10937-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10937-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="10937-165">Response</span></span>

<span data-ttu-id="10937-166">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos de [inscrição](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10937-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10937-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10937-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="10937-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10937-168">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="10937-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="10937-169">Response</span></span>

<span data-ttu-id="10937-170">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10937-170">Here is an example of the response.</span></span> <span data-ttu-id="10937-171">Observação: A resposta mostrada aqui pode estar truncada para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="10937-171">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="10937-172">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10937-172">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

<span data-ttu-id="10937-173">Quando uma solicitação retorna várias páginas de dados, a resposta inclui um `@odata.nextLink` propriedade para ajudá-lo a gerenciar os resultados.</span><span class="sxs-lookup"><span data-stu-id="10937-173">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="10937-174">Para saber mais, consulte [os dados de paginação Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="10937-174">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
