# <a name="list-subscriptions"></a><span data-ttu-id="325d6-101">Inscrições de lista</span><span class="sxs-lookup"><span data-stu-id="325d6-101">List subscriptions</span></span>

<span data-ttu-id="325d6-102">Recupere as propriedades e relacionamentos de inscrições de webhook, com base na função do usuário com um locatário, o usuário e a ID de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="325d6-102">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="325d6-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="325d6-103">Permissions</span></span>

<span data-ttu-id="325d6-104">Essa API suporta os seguintes escopos de permissão; Para saber mais, incluindo como escolher permissões, consulte [permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="325d6-104">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="325d6-105">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="325d6-105">Permission type</span></span>  | <span data-ttu-id="325d6-106">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="325d6-106">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="325d6-107">[Permissão delegadas](../../../concepts/auth_v2_user.md) (conta do trabalho ou da escola)</span><span class="sxs-lookup"><span data-stu-id="325d6-107">[Delegated permission](../../../concepts/auth_v2_user.md) (work or school account)</span></span> | <span data-ttu-id="325d6-108">Função exigida para [criar a inscrição](subscription_post_subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="325d6-108">Role required to [create subscription](subscription_post_subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="325d6-109">[Permissão delegadas](../../../concepts/auth_v2_user.md) (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="325d6-109">[Delegated permission](../../../concepts/auth_v2_user.md) (personal Microsoft account)</span></span> | <span data-ttu-id="325d6-110">Função exigida para [criar a inscrição](subscription_post_subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="325d6-110">Role required to [create subscription](subscription_post_subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="325d6-111">Permissão de aplicativo</span><span class="sxs-lookup"><span data-stu-id="325d6-111">Application permission</span></span>](../../../concepts/auth_v2_service.md) | <span data-ttu-id="325d6-112">Função necessária para [criar a assinatura](subscription_post_subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="325d6-112">Role required to [create subscription](subscription_post_subscriptions.md).</span></span> |

<span data-ttu-id="325d6-113">Resultados de resposta são baseados no contexto do aplicativo chamado.</span><span class="sxs-lookup"><span data-stu-id="325d6-113">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="325d6-114">Apresentamos a seguir um resumo dos cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="325d6-114">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="325d6-115">Cenários básicos</span><span class="sxs-lookup"><span data-stu-id="325d6-115">Basic scenarios</span></span>

<span data-ttu-id="325d6-116">Mais comumente, um aplicativo deseja recuperar as assinaturas que originalmente criado para o usuário conectado no momento, ou para todos os usuários no diretório (contas de trabalho/escola).</span><span class="sxs-lookup"><span data-stu-id="325d6-116">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="325d6-117">Esses cenários não exigem qualquer permissões especiais além do aplicativo originalmente usado para criar suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="325d6-117">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="325d6-118">Contexto do aplicativo chamado</span><span class="sxs-lookup"><span data-stu-id="325d6-118">Context of the calling app</span></span> | <span data-ttu-id="325d6-119">Resposta conterá</span><span class="sxs-lookup"><span data-stu-id="325d6-119">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="325d6-120">App está chamando em nome do usuário conectado (delegada permissão).</span><span class="sxs-lookup"><span data-stu-id="325d6-120">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="325d6-121">- e -</span><span class="sxs-lookup"><span data-stu-id="325d6-121">-and-</span></span><br/><span data-ttu-id="325d6-122">App tem a permissão original necessária para [criar a assinatura](subscription_post_subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="325d6-122">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="325d6-123">Observação: Isso se aplica ao pessoais contas da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="325d6-123">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="325d6-124">Inscrições criadas por **Este aplicativo** para o usuário entrou no apenas.</span><span class="sxs-lookup"><span data-stu-id="325d6-124">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="325d6-125">App está chamando em nome do próprio (permissão de aplicativo).</span><span class="sxs-lookup"><span data-stu-id="325d6-125">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="325d6-126">- e -</span><span class="sxs-lookup"><span data-stu-id="325d6-126">-and-</span></span><br/><span data-ttu-id="325d6-127">App tem a permissão original necessária para [criar a assinatura](subscription_post_subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="325d6-127">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="325d6-128">Observação: Isso se aplica a apenas contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="325d6-128">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="325d6-129">Inscrições criadas por **Este aplicativo** para si mesmo ou para qualquer usuário no diretório.</span><span class="sxs-lookup"><span data-stu-id="325d6-129">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="325d6-130">Cenários avançados</span><span class="sxs-lookup"><span data-stu-id="325d6-130">Advanced scenarios</span></span>

<span data-ttu-id="325d6-131">Em alguns casos, um aplicativo quer recuperar inscrições criadas por outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="325d6-131">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="325d6-132">Por exemplo, um usuário quiser ver todas as inscrições criadas por qualquer aplicativo em nome deles.</span><span class="sxs-lookup"><span data-stu-id="325d6-132">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="325d6-133">Ou então, um administrador talvez queira ver todas as inscrições de todos os aplicativos no seu diretório.</span><span class="sxs-lookup"><span data-stu-id="325d6-133">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="325d6-134">Para nesses cenários, uma permissão delegada Subscription.Read.All é necessária.</span><span class="sxs-lookup"><span data-stu-id="325d6-134">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="325d6-135">Contexto do aplicativo chamado</span><span class="sxs-lookup"><span data-stu-id="325d6-135">Context of the calling app</span></span> | <span data-ttu-id="325d6-136">Resposta conterá</span><span class="sxs-lookup"><span data-stu-id="325d6-136">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="325d6-137">App está chamando em nome do usuário conectado (delegada permissão).</span><span class="sxs-lookup"><span data-stu-id="325d6-137">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="325d6-138">*O usuário é um não seja o administrador*.</span><span class="sxs-lookup"><span data-stu-id="325d6-138">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="325d6-139">- e -</span><span class="sxs-lookup"><span data-stu-id="325d6-139">-and-</span></span><br/><span data-ttu-id="325d6-140">App tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="325d6-140">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="325d6-141">Observação: Isso se aplica ao pessoais contas da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="325d6-141">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="325d6-142">Inscrições criadas por **qualquer aplicativo** para o usuário entrou no apenas.</span><span class="sxs-lookup"><span data-stu-id="325d6-142">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="325d6-143">App está chamando em nome do usuário conectado (delegada permissão).</span><span class="sxs-lookup"><span data-stu-id="325d6-143">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="325d6-144">*O usuário é um administrador*.</span><span class="sxs-lookup"><span data-stu-id="325d6-144">*The user is an admin*.</span></span><br/><span data-ttu-id="325d6-145">- e -</span><span class="sxs-lookup"><span data-stu-id="325d6-145">-and-</span></span><br/><span data-ttu-id="325d6-146">App tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="325d6-146">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="325d6-147">Observação: Isso se aplica a apenas contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="325d6-147">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="325d6-148">Inscrições criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.</span><span class="sxs-lookup"><span data-stu-id="325d6-148">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="325d6-149">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="325d6-149">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="325d6-150">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="325d6-150">Optional query parameters</span></span>

<span data-ttu-id="325d6-151">Este método não oferece suporte para os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="325d6-151">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="325d6-152">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="325d6-152">Request headers</span></span>

| <span data-ttu-id="325d6-153">Nome</span><span class="sxs-lookup"><span data-stu-id="325d6-153">Name</span></span>       | <span data-ttu-id="325d6-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="325d6-154">Type</span></span> | <span data-ttu-id="325d6-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="325d6-155">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="325d6-156">Autorização</span><span class="sxs-lookup"><span data-stu-id="325d6-156">Authorization</span></span>  | <span data-ttu-id="325d6-157">string</span><span class="sxs-lookup"><span data-stu-id="325d6-157">string</span></span>  | <span data-ttu-id="325d6-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="325d6-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="325d6-160">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="325d6-160">Request body</span></span>

<span data-ttu-id="325d6-161">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="325d6-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="325d6-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="325d6-162">Response</span></span>

<span data-ttu-id="325d6-163">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos de [inscrição](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="325d6-163">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="325d6-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="325d6-164">Example</span></span>

##### <a name="request"></a><span data-ttu-id="325d6-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="325d6-165">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="325d6-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="325d6-166">Response</span></span>

<span data-ttu-id="325d6-167">Aqui está um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="325d6-167">Here's an an example of the response.</span></span>  <span data-ttu-id="325d6-168">Observe que ele pode estar truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="325d6-168">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="325d6-169">Todas as propriedades apropriadas para a solicitação de compatíveis e o contexto de chamada será retornado de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="325d6-169">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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

<span data-ttu-id="325d6-170">Quando uma solicitação retorna várias páginas de dados, a resposta inclui um `@odata.nextLink` propriedade para ajudá-lo a gerenciar os resultados.</span><span class="sxs-lookup"><span data-stu-id="325d6-170">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="325d6-171">Para saber mais, consulte [os dados de paginação Microsoft Graph em seu aplicativo](../../../concepts/paging.md).</span><span class="sxs-lookup"><span data-stu-id="325d6-171">To learn more, see [Paging Microsoft Graph data in your app](../../../concepts/paging.md).</span></span>
