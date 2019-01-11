---
title: Inscrições de lista
description: Recupere as propriedades e relacionamentos de inscrições de webhook, com base na função do usuário com um locatário, o usuário e a ID de aplicativo.
localization_priority: Priority
ms.openlocfilehash: 663586cc769f04be631e1f3c1bdf86bc4f798022
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850411"
---
# <a name="list-subscriptions"></a><span data-ttu-id="331d9-103">Inscrições de lista</span><span class="sxs-lookup"><span data-stu-id="331d9-103">List subscriptions</span></span>

<span data-ttu-id="331d9-104">Recupere as propriedades e relacionamentos de inscrições de webhook, com base na função do usuário com um locatário, o usuário e a ID de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="331d9-104">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="331d9-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="331d9-105">Permissions</span></span>

<span data-ttu-id="331d9-106">Essa API suporta os seguintes escopos de permissão; Para saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="331d9-106">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="331d9-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="331d9-107">Permission type</span></span>  | <span data-ttu-id="331d9-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="331d9-108">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="331d9-109">[Permissão delegadas](/graph/auth-v2-user) (conta do trabalho ou da escola)</span><span class="sxs-lookup"><span data-stu-id="331d9-109">[Delegated permission](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="331d9-110">Função exigida para [criar a inscrição](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="331d9-110">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="331d9-111">[Permissão delegadas](/graph/auth-v2-user) (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="331d9-111">[Delegated permission](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="331d9-112">Função exigida para [criar a inscrição](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="331d9-112">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="331d9-113">Permissão de aplicativo</span><span class="sxs-lookup"><span data-stu-id="331d9-113">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="331d9-114">Função necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="331d9-114">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="331d9-115">Resultados de resposta são baseados no contexto do aplicativo chamado.</span><span class="sxs-lookup"><span data-stu-id="331d9-115">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="331d9-116">Apresentamos a seguir um resumo dos cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="331d9-116">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="331d9-117">Cenários básicos</span><span class="sxs-lookup"><span data-stu-id="331d9-117">Basic scenarios</span></span>

<span data-ttu-id="331d9-118">Mais comumente, um aplicativo deseja recuperar as assinaturas que originalmente criado para o usuário conectado no momento, ou para todos os usuários no diretório (contas de trabalho/escola).</span><span class="sxs-lookup"><span data-stu-id="331d9-118">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="331d9-119">Esses cenários não exigem qualquer permissões especiais além do aplicativo originalmente usado para criar suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="331d9-119">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="331d9-120">Contexto do aplicativo chamado</span><span class="sxs-lookup"><span data-stu-id="331d9-120">Context of the calling app</span></span> | <span data-ttu-id="331d9-121">Resposta conterá</span><span class="sxs-lookup"><span data-stu-id="331d9-121">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="331d9-122">App está chamando em nome do usuário conectado (delegada permissão).</span><span class="sxs-lookup"><span data-stu-id="331d9-122">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="331d9-123">- e -</span><span class="sxs-lookup"><span data-stu-id="331d9-123">-and-</span></span><br/><span data-ttu-id="331d9-124">App tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="331d9-124">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="331d9-125">Observação: Isso se aplica ao pessoais contas da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="331d9-125">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="331d9-126">Inscrições criadas por **Este aplicativo** para o usuário entrou no apenas.</span><span class="sxs-lookup"><span data-stu-id="331d9-126">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="331d9-127">App está chamando em nome do próprio (permissão de aplicativo).</span><span class="sxs-lookup"><span data-stu-id="331d9-127">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="331d9-128">- e -</span><span class="sxs-lookup"><span data-stu-id="331d9-128">-and-</span></span><br/><span data-ttu-id="331d9-129">App tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="331d9-129">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="331d9-130">Observação: Isso se aplica a apenas contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="331d9-130">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="331d9-131">Inscrições criadas por **Este aplicativo** para si mesmo ou para qualquer usuário no diretório.</span><span class="sxs-lookup"><span data-stu-id="331d9-131">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="331d9-132">Cenários avançados</span><span class="sxs-lookup"><span data-stu-id="331d9-132">Advanced scenarios</span></span>

<span data-ttu-id="331d9-133">Em alguns casos, um aplicativo quer recuperar inscrições criadas por outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="331d9-133">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="331d9-134">Por exemplo, um usuário quiser ver todas as inscrições criadas por qualquer aplicativo em nome deles.</span><span class="sxs-lookup"><span data-stu-id="331d9-134">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="331d9-135">Ou então, um administrador talvez queira ver todas as inscrições de todos os aplicativos no seu diretório.</span><span class="sxs-lookup"><span data-stu-id="331d9-135">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="331d9-136">Para nesses cenários, uma permissão delegada Subscription.Read.All é necessária.</span><span class="sxs-lookup"><span data-stu-id="331d9-136">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="331d9-137">Contexto do aplicativo chamado</span><span class="sxs-lookup"><span data-stu-id="331d9-137">Context of the calling app</span></span> | <span data-ttu-id="331d9-138">Resposta conterá</span><span class="sxs-lookup"><span data-stu-id="331d9-138">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="331d9-139">App está chamando em nome do usuário conectado (delegada permissão).</span><span class="sxs-lookup"><span data-stu-id="331d9-139">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="331d9-140">*O usuário é um não seja o administrador*.</span><span class="sxs-lookup"><span data-stu-id="331d9-140">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="331d9-141">- e -</span><span class="sxs-lookup"><span data-stu-id="331d9-141">-and-</span></span><br/><span data-ttu-id="331d9-142">App tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="331d9-142">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="331d9-143">Observação: Isso se aplica ao pessoais contas da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="331d9-143">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="331d9-144">Inscrições criadas por **qualquer aplicativo** para o usuário entrou no apenas.</span><span class="sxs-lookup"><span data-stu-id="331d9-144">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="331d9-145">App está chamando em nome do usuário conectado (delegada permissão).</span><span class="sxs-lookup"><span data-stu-id="331d9-145">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="331d9-146">*O usuário é um administrador*.</span><span class="sxs-lookup"><span data-stu-id="331d9-146">*The user is an admin*.</span></span><br/><span data-ttu-id="331d9-147">- e -</span><span class="sxs-lookup"><span data-stu-id="331d9-147">-and-</span></span><br/><span data-ttu-id="331d9-148">App tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="331d9-148">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="331d9-149">Observação: Isso se aplica a apenas contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="331d9-149">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="331d9-150">Inscrições criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.</span><span class="sxs-lookup"><span data-stu-id="331d9-150">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="331d9-151">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="331d9-151">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="331d9-152">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="331d9-152">Optional query parameters</span></span>

<span data-ttu-id="331d9-153">Este método não oferece suporte para os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="331d9-153">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="331d9-154">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="331d9-154">Request headers</span></span>

| <span data-ttu-id="331d9-155">Nome</span><span class="sxs-lookup"><span data-stu-id="331d9-155">Name</span></span>       | <span data-ttu-id="331d9-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="331d9-156">Type</span></span> | <span data-ttu-id="331d9-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="331d9-157">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="331d9-158">Autorização</span><span class="sxs-lookup"><span data-stu-id="331d9-158">Authorization</span></span>  | <span data-ttu-id="331d9-159">string</span><span class="sxs-lookup"><span data-stu-id="331d9-159">string</span></span>  | <span data-ttu-id="331d9-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="331d9-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="331d9-162">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="331d9-162">Request body</span></span>

<span data-ttu-id="331d9-163">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="331d9-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="331d9-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="331d9-164">Response</span></span>

<span data-ttu-id="331d9-165">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos de [inscrição](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="331d9-165">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="331d9-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="331d9-166">Example</span></span>

##### <a name="request"></a><span data-ttu-id="331d9-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="331d9-167">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="331d9-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="331d9-168">Response</span></span>

<span data-ttu-id="331d9-169">Aqui está um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="331d9-169">Here's an an example of the response.</span></span>  <span data-ttu-id="331d9-170">Observe que ele pode estar truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="331d9-170">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="331d9-171">Todas as propriedades apropriadas para a solicitação de compatíveis e o contexto de chamada será retornado de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="331d9-171">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions",
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
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

<span data-ttu-id="331d9-172">Quando uma solicitação retorna várias páginas de dados, a resposta inclui um `@odata.nextLink` propriedade para ajudá-lo a gerenciar os resultados.</span><span class="sxs-lookup"><span data-stu-id="331d9-172">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="331d9-173">Para saber mais, consulte [os dados de paginação Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="331d9-173">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
