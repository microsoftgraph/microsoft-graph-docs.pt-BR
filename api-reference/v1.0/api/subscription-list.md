---
title: Listar assinaturas
description: Recupere as propriedades e os relacionamentos das assinaturas do webhook, com base no ID do aplicativo, no usuário e na função do usuário com um locatário.
localization_priority: Priority
author: Jumaodhiss
ms.prod: change-notifications
doc_type: apiPageType
ms.openlocfilehash: cd5c72305e070745407c2c89cc5213758ce591b3
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468841"
---
# <a name="list-subscriptions"></a><span data-ttu-id="9cb8a-103">Listar assinaturas</span><span class="sxs-lookup"><span data-stu-id="9cb8a-103">List subscriptions</span></span>

<span data-ttu-id="9cb8a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cb8a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9cb8a-105">Recupere as propriedades e os relacionamentos das assinaturas do webhook, com base no ID do aplicativo, no usuário e na função do usuário com um locatário.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-105">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cb8a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9cb8a-106">Permissions</span></span>

<span data-ttu-id="9cb8a-107">Esta API suporta os seguintes escopos de permissão; para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cb8a-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9cb8a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cb8a-108">Permission type</span></span>  | <span data-ttu-id="9cb8a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9cb8a-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="9cb8a-110">[Permissão delegada](/graph/auth-v2-user) (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cb8a-110">[Delegated permission](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="9cb8a-111">Função necessária para [criar assinatura](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="9cb8a-111">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="9cb8a-112">[Permissão delegada](/graph/auth-v2-user) (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cb8a-112">[Delegated permission](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="9cb8a-113">Função necessária para [criar assinatura](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="9cb8a-113">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="9cb8a-114">Permissão de aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cb8a-114">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="9cb8a-115">Função necessária para [criar assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="9cb8a-115">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="9cb8a-116">Os resultados da resposta são baseados no contexto do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="9cb8a-117">A seguir, um resumo dos cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="9cb8a-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="9cb8a-118">Cenários Básicos</span><span class="sxs-lookup"><span data-stu-id="9cb8a-118">Basic scenarios</span></span>

<span data-ttu-id="9cb8a-119">Comumente, um aplicativo deseja recuperar assinaturas originalmente criadas para o usuário atualmente conectado ou para todos os usuários no diretório (contas corporativas/de estudante).</span><span class="sxs-lookup"><span data-stu-id="9cb8a-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="9cb8a-120">Esses cenários não exigem permissões especiais além daquelas usadas originalmente pelo aplicativo para criar suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="9cb8a-121">Contexto do aplicativo de chamada</span><span class="sxs-lookup"><span data-stu-id="9cb8a-121">Context of the calling app</span></span> | <span data-ttu-id="9cb8a-122">A resposta contém</span><span class="sxs-lookup"><span data-stu-id="9cb8a-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="9cb8a-123">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="9cb8a-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="9cb8a-124">-e-</span><span class="sxs-lookup"><span data-stu-id="9cb8a-124">-and-</span></span><br/><span data-ttu-id="9cb8a-125">O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="9cb8a-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="9cb8a-126">Nota: Isso se aplica a contas pessoais da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="9cb8a-127">Assinaturas criadas por **este aplicativo** apenas para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="9cb8a-128">O aplicativo está chamando em nome de si mesmo (permissão de aplicativo).</span><span class="sxs-lookup"><span data-stu-id="9cb8a-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="9cb8a-129">-e-</span><span class="sxs-lookup"><span data-stu-id="9cb8a-129">-and-</span></span><br/><span data-ttu-id="9cb8a-130">O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="9cb8a-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="9cb8a-131">Nota: Isso se aplica apenas a contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="9cb8a-132">Assinaturas criadas por **este aplicativo** para si ou para qualquer usuário no diretório.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="9cb8a-133">Cenários avançados</span><span class="sxs-lookup"><span data-stu-id="9cb8a-133">Advanced scenarios</span></span>

<span data-ttu-id="9cb8a-134">Em alguns casos, um aplicativo deseja recuperar assinaturas criadas por outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="9cb8a-135">Por exemplo, um usuário deseja ver todas as assinaturas criadas por qualquer aplicativo em seu nome.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="9cb8a-136">Ou, um administrador pode querer ver todas as assinaturas de todos os aplicativos em seu diretório.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="9cb8a-137">Para esses cenários, é necessária uma permissão delegada Subscription.Read.All.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="9cb8a-138">Contexto do aplicativo de chamada</span><span class="sxs-lookup"><span data-stu-id="9cb8a-138">Context of the calling app</span></span> | <span data-ttu-id="9cb8a-139">A resposta contém</span><span class="sxs-lookup"><span data-stu-id="9cb8a-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="9cb8a-140">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="9cb8a-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="9cb8a-141">*O usuário é um não administrador*.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="9cb8a-142">-e-</span><span class="sxs-lookup"><span data-stu-id="9cb8a-142">-and-</span></span><br/><span data-ttu-id="9cb8a-143">O aplicativo tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cb8a-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="9cb8a-144">Nota: Isso se aplica a contas pessoais da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="9cb8a-145">Assinaturas criadas por **qualquer aplicativo** apenas para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="9cb8a-146">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="9cb8a-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="9cb8a-147">*O usuário é um administrador*.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-147">*The user is an admin*.</span></span><br/><span data-ttu-id="9cb8a-148">-e-</span><span class="sxs-lookup"><span data-stu-id="9cb8a-148">-and-</span></span><br/><span data-ttu-id="9cb8a-149">O aplicativo tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cb8a-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="9cb8a-150">Nota: Isso se aplica apenas a contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="9cb8a-151">Assinaturas criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cb8a-152">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cb8a-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9cb8a-153">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9cb8a-153">Optional query parameters</span></span>

<span data-ttu-id="9cb8a-154">Este método não é compatível com os [Parâmetros de Consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-154">This method does not support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9cb8a-155">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cb8a-155">Request headers</span></span>

| <span data-ttu-id="9cb8a-156">Nome</span><span class="sxs-lookup"><span data-stu-id="9cb8a-156">Name</span></span>       | <span data-ttu-id="9cb8a-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cb8a-157">Type</span></span> | <span data-ttu-id="9cb8a-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cb8a-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9cb8a-159">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cb8a-159">Authorization</span></span>  | <span data-ttu-id="9cb8a-160">string</span><span class="sxs-lookup"><span data-stu-id="9cb8a-160">string</span></span>  | <span data-ttu-id="9cb8a-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cb8a-163">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cb8a-163">Request body</span></span>

<span data-ttu-id="9cb8a-164">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cb8a-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cb8a-165">Response</span></span>

<span data-ttu-id="9cb8a-166">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma lista de objetos de [assinatura](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cb8a-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cb8a-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9cb8a-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cb8a-168">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9cb8a-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cb8a-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions
```
# <a name="c"></a>[<span data-ttu-id="9cb8a-170">C#</span><span class="sxs-lookup"><span data-stu-id="9cb8a-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cb8a-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cb8a-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cb8a-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cb8a-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cb8a-173">Java</span><span class="sxs-lookup"><span data-stu-id="9cb8a-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9cb8a-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cb8a-174">Response</span></span>

<span data-ttu-id="9cb8a-175">Veja um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-175">Here's an example of the response.</span></span>  <span data-ttu-id="9cb8a-176">Observe que pode estar truncada, para brevidade.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-176">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="9cb8a-177">Todas as propriedades compatíveis apropriadas para a solicitação e contexto de chamada serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-177">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
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
      "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
      "latestSupportedTlsVersion": "v1_2",
      "encryptionCertificate": "",
      "encryptionCertificateId": "",
      "includeResourceData": false,
      "notificationContentType": "application/json"
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

> <span data-ttu-id="9cb8a-178">**Observação:** o valor da propriedade `clientState` não é retornado para fins de segurança.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-178">**Note:** the `clientState` property value is not returned for security purposes.</span></span>  

<span data-ttu-id="9cb8a-179">Quando uma solicitação retorna várias páginas de dados, a resposta inclui uma propriedade `@odata.nextLink` para ajudá-lo a gerenciar os resultados.</span><span class="sxs-lookup"><span data-stu-id="9cb8a-179">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="9cb8a-180">Para saber mais, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="9cb8a-180">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
