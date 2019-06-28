---
title: Listar assinaturas
description: Recupere as propriedades e os relacionamentos das assinaturas do webhook, com base no ID do aplicativo, no usuário e na função do usuário com um locatário.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 603a918faa9153f4b8690613a2b9aed7b7f53420
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273140"
---
# <a name="list-subscriptions"></a><span data-ttu-id="864a3-103">Listar assinaturas</span><span class="sxs-lookup"><span data-stu-id="864a3-103">List subscriptions</span></span>

<span data-ttu-id="864a3-104">Recupere as propriedades e os relacionamentos das assinaturas do webhook, com base no ID do aplicativo, no usuário e na função do usuário com um locatário.</span><span class="sxs-lookup"><span data-stu-id="864a3-104">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="864a3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="864a3-105">Permissions</span></span>

<span data-ttu-id="864a3-106">Esta API suporta os seguintes escopos de permissão; para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="864a3-106">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="864a3-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="864a3-107">Permission type</span></span>  | <span data-ttu-id="864a3-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="864a3-108">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="864a3-109">[Permissão delegada](/graph/auth-v2-user) (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="864a3-109">[Delegated permission](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="864a3-110">Função necessária para [criar assinatura](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="864a3-110">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="864a3-111">[Permissão delegada](/graph/auth-v2-user) (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="864a3-111">[Delegated permission](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="864a3-112">Função necessária para [criar assinatura](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="864a3-112">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="864a3-113">Permissão de aplicativo</span><span class="sxs-lookup"><span data-stu-id="864a3-113">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="864a3-114">Função necessária para [criar assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="864a3-114">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="864a3-115">Os resultados da resposta são baseados no contexto do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="864a3-115">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="864a3-116">A seguir, um resumo dos cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="864a3-116">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="864a3-117">Cenários Básicos</span><span class="sxs-lookup"><span data-stu-id="864a3-117">Basic scenarios</span></span>

<span data-ttu-id="864a3-118">Comumente, um aplicativo deseja recuperar assinaturas originalmente criadas para o usuário atualmente conectado ou para todos os usuários no diretório (contas corporativas/de estudante).</span><span class="sxs-lookup"><span data-stu-id="864a3-118">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="864a3-119">Esses cenários não exigem permissões especiais além daquelas usadas originalmente pelo aplicativo para criar suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="864a3-119">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="864a3-120">Contexto do aplicativo de chamada</span><span class="sxs-lookup"><span data-stu-id="864a3-120">Context of the calling app</span></span> | <span data-ttu-id="864a3-121">A resposta contém</span><span class="sxs-lookup"><span data-stu-id="864a3-121">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="864a3-122">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="864a3-122">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="864a3-123">-e-</span><span class="sxs-lookup"><span data-stu-id="864a3-123">-and-</span></span><br/><span data-ttu-id="864a3-124">O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="864a3-124">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="864a3-125">Nota: Isso se aplica a contas pessoais da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="864a3-125">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="864a3-126">Assinaturas criadas por **este aplicativo** apenas para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="864a3-126">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="864a3-127">O aplicativo está chamando em nome de si mesmo (permissão de aplicativo).</span><span class="sxs-lookup"><span data-stu-id="864a3-127">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="864a3-128">-e-</span><span class="sxs-lookup"><span data-stu-id="864a3-128">-and-</span></span><br/><span data-ttu-id="864a3-129">O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="864a3-129">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="864a3-130">Nota: Isso se aplica apenas a contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="864a3-130">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="864a3-131">Assinaturas criadas por **este aplicativo** para si ou para qualquer usuário no diretório.</span><span class="sxs-lookup"><span data-stu-id="864a3-131">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="864a3-132">Cenários avançados</span><span class="sxs-lookup"><span data-stu-id="864a3-132">Advanced scenarios</span></span>

<span data-ttu-id="864a3-133">Em alguns casos, um aplicativo deseja recuperar assinaturas criadas por outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="864a3-133">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="864a3-134">Por exemplo, um usuário deseja ver todas as assinaturas criadas por qualquer aplicativo em seu nome.</span><span class="sxs-lookup"><span data-stu-id="864a3-134">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="864a3-135">Ou, um administrador pode querer ver todas as assinaturas de todos os aplicativos em seu diretório.</span><span class="sxs-lookup"><span data-stu-id="864a3-135">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="864a3-136">Para esses cenários, é necessária uma permissão delegada Subscription.Read.All.</span><span class="sxs-lookup"><span data-stu-id="864a3-136">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="864a3-137">Contexto do aplicativo de chamada</span><span class="sxs-lookup"><span data-stu-id="864a3-137">Context of the calling app</span></span> | <span data-ttu-id="864a3-138">A resposta contém</span><span class="sxs-lookup"><span data-stu-id="864a3-138">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="864a3-139">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="864a3-139">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="864a3-140">*O usuário é um não administrador*.</span><span class="sxs-lookup"><span data-stu-id="864a3-140">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="864a3-141">-e-</span><span class="sxs-lookup"><span data-stu-id="864a3-141">-and-</span></span><br/><span data-ttu-id="864a3-142">O aplicativo tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="864a3-142">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="864a3-143">Nota: Isso se aplica a contas pessoais da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="864a3-143">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="864a3-144">Assinaturas criadas por **qualquer aplicativo** apenas para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="864a3-144">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="864a3-145">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="864a3-145">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="864a3-146">*O usuário é um administrador*.</span><span class="sxs-lookup"><span data-stu-id="864a3-146">*The user is an admin*.</span></span><br/><span data-ttu-id="864a3-147">-e-</span><span class="sxs-lookup"><span data-stu-id="864a3-147">-and-</span></span><br/><span data-ttu-id="864a3-148">O aplicativo tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="864a3-148">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="864a3-149">Nota: Isso se aplica apenas a contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="864a3-149">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="864a3-150">Assinaturas criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.</span><span class="sxs-lookup"><span data-stu-id="864a3-150">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="864a3-151">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="864a3-151">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="864a3-152">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="864a3-152">Optional query parameters</span></span>

<span data-ttu-id="864a3-153">Este método não é compatível com os [Parâmetros de Consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="864a3-153">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="864a3-154">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="864a3-154">Request headers</span></span>

| <span data-ttu-id="864a3-155">Nome</span><span class="sxs-lookup"><span data-stu-id="864a3-155">Name</span></span>       | <span data-ttu-id="864a3-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="864a3-156">Type</span></span> | <span data-ttu-id="864a3-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="864a3-157">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="864a3-158">Autorização</span><span class="sxs-lookup"><span data-stu-id="864a3-158">Authorization</span></span>  | <span data-ttu-id="864a3-159">string</span><span class="sxs-lookup"><span data-stu-id="864a3-159">string</span></span>  | <span data-ttu-id="864a3-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="864a3-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="864a3-162">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="864a3-162">Request body</span></span>

<span data-ttu-id="864a3-163">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="864a3-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="864a3-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="864a3-164">Response</span></span>

<span data-ttu-id="864a3-165">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma lista de objetos de [assinatura](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="864a3-165">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="864a3-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="864a3-166">Example</span></span>

##### <a name="request"></a><span data-ttu-id="864a3-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="864a3-167">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="864a3-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="864a3-168">Response</span></span>

<span data-ttu-id="864a3-169">Aqui está um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="864a3-169">Here's an an example of the response.</span></span>  <span data-ttu-id="864a3-170">Observe que pode estar truncada, para brevidade.</span><span class="sxs-lookup"><span data-stu-id="864a3-170">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="864a3-171">Todas as propriedades compatíveis apropriadas para a solicitação e contexto de chamada serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="864a3-171">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="864a3-172">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="864a3-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="864a3-173">C#</span><span class="sxs-lookup"><span data-stu-id="864a3-173">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscriptions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="864a3-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="864a3-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscriptions-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="864a3-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="864a3-175">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_subscriptions-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

<span data-ttu-id="864a3-176">Quando uma solicitação retorna várias páginas de dados, a resposta inclui uma propriedade `@odata.nextLink` para ajudá-lo a gerenciar os resultados.</span><span class="sxs-lookup"><span data-stu-id="864a3-176">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="864a3-177">Para saber mais, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="864a3-177">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
