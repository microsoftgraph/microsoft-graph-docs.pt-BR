---
title: Listar assinaturas
description: " Veja os cenários abaixo para obter detalhes."
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: d48036e3c54d0014abf6676877a329bcb81964e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453153"
---
# <a name="list-subscriptions"></a><span data-ttu-id="adb35-103">Listar assinaturas</span><span class="sxs-lookup"><span data-stu-id="adb35-103">List subscriptions</span></span>

<span data-ttu-id="adb35-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="adb35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adb35-105">Recupere uma lista de assinaturas de webhook.</span><span class="sxs-lookup"><span data-stu-id="adb35-105">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="adb35-106">O conteúdo da resposta depende do contexto no qual o aplicativo está chamando; Veja os cenários abaixo para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="adb35-106">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="adb35-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="adb35-107">Permissions</span></span>

<span data-ttu-id="adb35-108">Esta API suporta os seguintes escopos de permissão; para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adb35-108">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="adb35-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adb35-109">Permission type</span></span>  | <span data-ttu-id="adb35-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="adb35-110">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="adb35-111">[Delegado](/graph/auth-v2-user) (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adb35-111">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="adb35-112">Permissão necessária para [criar assinatura](subscription-post-subscriptions.md) ou assinatura. Read. All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="adb35-112">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="adb35-113">[Delegado](/graph/auth-v2-user) (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adb35-113">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="adb35-114">Permissão necessária para [criar assinatura](subscription-post-subscriptions.md) ou assinatura. Read. All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="adb35-114">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="adb35-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adb35-115">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="adb35-116">Permissão necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="adb35-116">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="adb35-117">Os resultados da resposta são baseados no contexto do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="adb35-117">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="adb35-118">A seguir, um resumo dos cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="adb35-118">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="adb35-119">Cenários Básicos</span><span class="sxs-lookup"><span data-stu-id="adb35-119">Basic scenarios</span></span>

<span data-ttu-id="adb35-120">Comumente, um aplicativo deseja recuperar assinaturas originalmente criadas para o usuário atualmente conectado ou para todos os usuários no diretório (contas corporativas/de estudante).</span><span class="sxs-lookup"><span data-stu-id="adb35-120">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="adb35-121">Esses cenários não exigem permissões especiais além daquelas usadas originalmente pelo aplicativo para criar suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="adb35-121">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="adb35-122">Contexto do aplicativo de chamada</span><span class="sxs-lookup"><span data-stu-id="adb35-122">Context of the calling app</span></span> | <span data-ttu-id="adb35-123">A resposta contém</span><span class="sxs-lookup"><span data-stu-id="adb35-123">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="adb35-124">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="adb35-124">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="adb35-125">-e-</span><span class="sxs-lookup"><span data-stu-id="adb35-125">-and-</span></span><br/><span data-ttu-id="adb35-126">O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="adb35-126">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="adb35-127">Nota: Isso se aplica a contas pessoais da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="adb35-127">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="adb35-128">Assinaturas criadas por **este aplicativo** apenas para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="adb35-128">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="adb35-129">O aplicativo está chamando em nome de si mesmo (permissão de aplicativo).</span><span class="sxs-lookup"><span data-stu-id="adb35-129">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="adb35-130">-e-</span><span class="sxs-lookup"><span data-stu-id="adb35-130">-and-</span></span><br/><span data-ttu-id="adb35-131">O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="adb35-131">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="adb35-132">Nota: Isso se aplica apenas a contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="adb35-132">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="adb35-133">Assinaturas criadas por **este aplicativo** para si ou para qualquer usuário no diretório.</span><span class="sxs-lookup"><span data-stu-id="adb35-133">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="adb35-134">Cenários avançados</span><span class="sxs-lookup"><span data-stu-id="adb35-134">Advanced scenarios</span></span>

<span data-ttu-id="adb35-135">Em alguns casos, um aplicativo deseja recuperar assinaturas criadas por outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="adb35-135">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="adb35-136">Por exemplo, um usuário deseja ver todas as assinaturas criadas por qualquer aplicativo em seu nome.</span><span class="sxs-lookup"><span data-stu-id="adb35-136">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="adb35-137">Ou, um administrador pode querer ver todas as assinaturas de todos os aplicativos em seu diretório.</span><span class="sxs-lookup"><span data-stu-id="adb35-137">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="adb35-138">Para esses cenários, é necessária uma permissão delegada Subscription.Read.All.</span><span class="sxs-lookup"><span data-stu-id="adb35-138">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="adb35-139">Contexto do aplicativo de chamada</span><span class="sxs-lookup"><span data-stu-id="adb35-139">Context of the calling app</span></span> | <span data-ttu-id="adb35-140">A resposta contém</span><span class="sxs-lookup"><span data-stu-id="adb35-140">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="adb35-141">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="adb35-141">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="adb35-142">*O usuário é um não administrador*.</span><span class="sxs-lookup"><span data-stu-id="adb35-142">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="adb35-143">-e-</span><span class="sxs-lookup"><span data-stu-id="adb35-143">-and-</span></span><br/><span data-ttu-id="adb35-144">O aplicativo tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="adb35-144">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="adb35-145">Nota: Isso se aplica a contas pessoais da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="adb35-145">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="adb35-146">Assinaturas criadas por **qualquer aplicativo** apenas para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="adb35-146">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="adb35-147">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="adb35-147">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="adb35-148">*O usuário é um administrador*.</span><span class="sxs-lookup"><span data-stu-id="adb35-148">*The user is an admin*.</span></span><br/><span data-ttu-id="adb35-149">-e-</span><span class="sxs-lookup"><span data-stu-id="adb35-149">-and-</span></span><br/><span data-ttu-id="adb35-150">O aplicativo tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="adb35-150">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="adb35-151">Nota: Isso se aplica apenas a contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="adb35-151">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="adb35-152">Assinaturas criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.</span><span class="sxs-lookup"><span data-stu-id="adb35-152">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adb35-153">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adb35-153">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="adb35-154">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="adb35-154">Optional query parameters</span></span>

<span data-ttu-id="adb35-155">Este método não é compatível com os [Parâmetros de Consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="adb35-155">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="adb35-156">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="adb35-156">Request headers</span></span>

| <span data-ttu-id="adb35-157">Nome</span><span class="sxs-lookup"><span data-stu-id="adb35-157">Name</span></span>       | <span data-ttu-id="adb35-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="adb35-158">Type</span></span> | <span data-ttu-id="adb35-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="adb35-159">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="adb35-160">Autorização</span><span class="sxs-lookup"><span data-stu-id="adb35-160">Authorization</span></span>  | <span data-ttu-id="adb35-161">string</span><span class="sxs-lookup"><span data-stu-id="adb35-161">string</span></span>  | <span data-ttu-id="adb35-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adb35-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adb35-164">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="adb35-164">Request body</span></span>

<span data-ttu-id="adb35-165">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="adb35-165">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adb35-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="adb35-166">Response</span></span>

<span data-ttu-id="adb35-167">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma lista de objetos de [assinatura](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="adb35-167">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adb35-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="adb35-168">Example</span></span>

##### <a name="request"></a><span data-ttu-id="adb35-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adb35-169">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="adb35-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="adb35-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions
```
# <a name="c"></a>[<span data-ttu-id="adb35-171">C#</span><span class="sxs-lookup"><span data-stu-id="adb35-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adb35-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adb35-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adb35-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adb35-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="adb35-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="adb35-174">Response</span></span>

<span data-ttu-id="adb35-175">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="adb35-175">Here is an example of the response.</span></span> <span data-ttu-id="adb35-176">Observação: a resposta mostrada aqui pode ser truncada por brevidade.</span><span class="sxs-lookup"><span data-stu-id="adb35-176">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="adb35-177">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="adb35-177">All of the properties will be returned from an actual call.</span></span>

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
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
      "latestSupportedTlsVersion": "v1_2"
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
  ]
}
-->

> <span data-ttu-id="adb35-178">**Observação:** o valor da propriedade `clientState` não é retornado para fins de segurança.</span><span class="sxs-lookup"><span data-stu-id="adb35-178">**Note:** the `clientState` property value is not returned for security purposes.</span></span>  

<span data-ttu-id="adb35-179">Quando uma solicitação retorna várias páginas de dados, a resposta inclui uma propriedade `@odata.nextLink` para ajudá-lo a gerenciar os resultados.</span><span class="sxs-lookup"><span data-stu-id="adb35-179">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="adb35-180">Para saber mais, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="adb35-180">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
