---
title: Listar assinaturas
description: Recupere as propriedades e os relacionamentos das assinaturas do webhook, com base no ID do aplicativo, no usuário e na função do usuário com um locatário.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 12377bccdc0e91b947541f32a614f412628c9b0e
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774923"
---
# <a name="list-subscriptions"></a><span data-ttu-id="23697-103">Listar assinaturas</span><span class="sxs-lookup"><span data-stu-id="23697-103">List subscriptions</span></span>

<span data-ttu-id="23697-104">Recupere as propriedades e os relacionamentos das assinaturas do webhook, com base no ID do aplicativo, no usuário e na função do usuário com um locatário.</span><span class="sxs-lookup"><span data-stu-id="23697-104">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="23697-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="23697-105">Permissions</span></span>

<span data-ttu-id="23697-106">Esta API suporta os seguintes escopos de permissão; para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23697-106">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23697-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23697-107">Permission type</span></span>  | <span data-ttu-id="23697-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23697-108">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="23697-109">[Permissão delegada](/graph/auth-v2-user) (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23697-109">[Delegated permission](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="23697-110">Função necessária para [criar assinatura](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="23697-110">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="23697-111">[Permissão delegada](/graph/auth-v2-user) (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23697-111">[Delegated permission](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="23697-112">Função necessária para [criar assinatura](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="23697-112">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="23697-113">Permissão de aplicativo</span><span class="sxs-lookup"><span data-stu-id="23697-113">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="23697-114">Função necessária para [criar assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="23697-114">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="23697-115">Os resultados da resposta são baseados no contexto do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="23697-115">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="23697-116">A seguir, um resumo dos cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="23697-116">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="23697-117">Cenários Básicos</span><span class="sxs-lookup"><span data-stu-id="23697-117">Basic scenarios</span></span>

<span data-ttu-id="23697-118">Comumente, um aplicativo deseja recuperar assinaturas originalmente criadas para o usuário atualmente conectado ou para todos os usuários no diretório (contas corporativas/de estudante).</span><span class="sxs-lookup"><span data-stu-id="23697-118">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="23697-119">Esses cenários não exigem permissões especiais além daquelas usadas originalmente pelo aplicativo para criar suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="23697-119">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="23697-120">Contexto do aplicativo de chamada</span><span class="sxs-lookup"><span data-stu-id="23697-120">Context of the calling app</span></span> | <span data-ttu-id="23697-121">A resposta contém</span><span class="sxs-lookup"><span data-stu-id="23697-121">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="23697-122">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="23697-122">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="23697-123">-e-</span><span class="sxs-lookup"><span data-stu-id="23697-123">-and-</span></span><br/><span data-ttu-id="23697-124">O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="23697-124">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="23697-125">Nota: Isso se aplica a contas pessoais da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="23697-125">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="23697-126">Assinaturas criadas por **este aplicativo** apenas para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="23697-126">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="23697-127">O aplicativo está chamando em nome de si mesmo (permissão de aplicativo).</span><span class="sxs-lookup"><span data-stu-id="23697-127">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="23697-128">-e-</span><span class="sxs-lookup"><span data-stu-id="23697-128">-and-</span></span><br/><span data-ttu-id="23697-129">O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="23697-129">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="23697-130">Nota: Isso se aplica apenas a contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="23697-130">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="23697-131">Assinaturas criadas por **este aplicativo** para si ou para qualquer usuário no diretório.</span><span class="sxs-lookup"><span data-stu-id="23697-131">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="23697-132">Cenários avançados</span><span class="sxs-lookup"><span data-stu-id="23697-132">Advanced scenarios</span></span>

<span data-ttu-id="23697-133">Em alguns casos, um aplicativo deseja recuperar assinaturas criadas por outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="23697-133">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="23697-134">Por exemplo, um usuário deseja ver todas as assinaturas criadas por qualquer aplicativo em seu nome.</span><span class="sxs-lookup"><span data-stu-id="23697-134">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="23697-135">Ou, um administrador pode querer ver todas as assinaturas de todos os aplicativos em seu diretório.</span><span class="sxs-lookup"><span data-stu-id="23697-135">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="23697-136">Para esses cenários, é necessária uma permissão delegada Subscription.Read.All.</span><span class="sxs-lookup"><span data-stu-id="23697-136">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="23697-137">Contexto do aplicativo de chamada</span><span class="sxs-lookup"><span data-stu-id="23697-137">Context of the calling app</span></span> | <span data-ttu-id="23697-138">A resposta contém</span><span class="sxs-lookup"><span data-stu-id="23697-138">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="23697-139">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="23697-139">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="23697-140">*O usuário é um não administrador*.</span><span class="sxs-lookup"><span data-stu-id="23697-140">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="23697-141">-e-</span><span class="sxs-lookup"><span data-stu-id="23697-141">-and-</span></span><br/><span data-ttu-id="23697-142">O aplicativo tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="23697-142">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="23697-143">Nota: Isso se aplica a contas pessoais da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="23697-143">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="23697-144">Assinaturas criadas por **qualquer aplicativo** apenas para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="23697-144">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="23697-145">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="23697-145">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="23697-146">*O usuário é um administrador*.</span><span class="sxs-lookup"><span data-stu-id="23697-146">*The user is an admin*.</span></span><br/><span data-ttu-id="23697-147">-e-</span><span class="sxs-lookup"><span data-stu-id="23697-147">-and-</span></span><br/><span data-ttu-id="23697-148">O aplicativo tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="23697-148">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="23697-149">Nota: Isso se aplica apenas a contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="23697-149">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="23697-150">Assinaturas criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.</span><span class="sxs-lookup"><span data-stu-id="23697-150">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23697-151">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23697-151">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23697-152">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="23697-152">Optional query parameters</span></span>

<span data-ttu-id="23697-153">Este método não é compatível com os [Parâmetros de Consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="23697-153">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23697-154">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23697-154">Request headers</span></span>

| <span data-ttu-id="23697-155">Nome</span><span class="sxs-lookup"><span data-stu-id="23697-155">Name</span></span>       | <span data-ttu-id="23697-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="23697-156">Type</span></span> | <span data-ttu-id="23697-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="23697-157">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="23697-158">Autorização</span><span class="sxs-lookup"><span data-stu-id="23697-158">Authorization</span></span>  | <span data-ttu-id="23697-159">string</span><span class="sxs-lookup"><span data-stu-id="23697-159">string</span></span>  | <span data-ttu-id="23697-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23697-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23697-162">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23697-162">Request body</span></span>

<span data-ttu-id="23697-163">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23697-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23697-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="23697-164">Response</span></span>

<span data-ttu-id="23697-165">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma lista de objetos de [assinatura](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23697-165">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23697-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23697-166">Example</span></span>

##### <a name="request"></a><span data-ttu-id="23697-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23697-167">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="23697-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="23697-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23697-169">C#</span><span class="sxs-lookup"><span data-stu-id="23697-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23697-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23697-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23697-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23697-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="23697-172">Java</span><span class="sxs-lookup"><span data-stu-id="23697-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="23697-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="23697-173">Response</span></span>

<span data-ttu-id="23697-174">Veja um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="23697-174">Here's an example of the response.</span></span>  <span data-ttu-id="23697-175">Observe que pode estar truncada, para brevidade.</span><span class="sxs-lookup"><span data-stu-id="23697-175">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="23697-176">Todas as propriedades compatíveis apropriadas para a solicitação e contexto de chamada serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23697-176">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
      "latestSupportedTlsVersion": "v1_2"
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

<span data-ttu-id="23697-177">Quando uma solicitação retorna várias páginas de dados, a resposta inclui uma propriedade `@odata.nextLink` para ajudá-lo a gerenciar os resultados.</span><span class="sxs-lookup"><span data-stu-id="23697-177">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="23697-178">Para saber mais, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="23697-178">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
