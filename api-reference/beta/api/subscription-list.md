---
title: Inscrições de lista
description: " Consulte os cenários abaixo para obter detalhes."
ms.openlocfilehash: ad5e97a9b721a9e557e01dd4743b53a52c6dc8d7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040073"
---
# <a name="list-subscriptions"></a><span data-ttu-id="bb96c-103">Inscrições de lista</span><span class="sxs-lookup"><span data-stu-id="bb96c-103">List subscriptions</span></span>

> <span data-ttu-id="bb96c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bb96c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb96c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bb96c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb96c-106">Recupere uma lista das inscrições de webhook.</span><span class="sxs-lookup"><span data-stu-id="bb96c-106">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="bb96c-107">O conteúdo da resposta depende do contexto no qual o aplicativo está chamando; Consulte os cenários abaixo para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="bb96c-107">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb96c-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="bb96c-108">Permissions</span></span>

<span data-ttu-id="bb96c-109">Essa API suporta os seguintes escopos de permissão; Para saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb96c-109">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb96c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb96c-110">Permission type</span></span>  | <span data-ttu-id="bb96c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb96c-111">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="bb96c-112">[Delegada](/graph/auth-v2-user) (conta do trabalho ou da escola)</span><span class="sxs-lookup"><span data-stu-id="bb96c-112">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="bb96c-113">Permissão necessária para [criar a inscrição](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="bb96c-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="bb96c-114">[Delegada](/graph/auth-v2-user) (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb96c-114">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="bb96c-115">Permissão necessária para [criar a inscrição](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="bb96c-115">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="bb96c-116">Application</span><span class="sxs-lookup"><span data-stu-id="bb96c-116">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="bb96c-117">Permissão necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="bb96c-117">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="bb96c-118">Resultados de resposta são baseados no contexto do aplicativo chamado.</span><span class="sxs-lookup"><span data-stu-id="bb96c-118">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="bb96c-119">Apresentamos a seguir um resumo dos cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="bb96c-119">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="bb96c-120">Cenários básicos</span><span class="sxs-lookup"><span data-stu-id="bb96c-120">Basic scenarios</span></span>

<span data-ttu-id="bb96c-121">Mais comumente, um aplicativo deseja recuperar as assinaturas que originalmente criado para o usuário conectado no momento, ou para todos os usuários no diretório (contas de trabalho/escola).</span><span class="sxs-lookup"><span data-stu-id="bb96c-121">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="bb96c-122">Esses cenários não exigem qualquer permissões especiais além do aplicativo originalmente usado para criar suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="bb96c-122">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="bb96c-123">Contexto do aplicativo chamado</span><span class="sxs-lookup"><span data-stu-id="bb96c-123">Context of the calling app</span></span> | <span data-ttu-id="bb96c-124">Resposta conterá</span><span class="sxs-lookup"><span data-stu-id="bb96c-124">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="bb96c-125">App está chamando em nome do usuário conectado (delegada permissão).</span><span class="sxs-lookup"><span data-stu-id="bb96c-125">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="bb96c-126">- e -</span><span class="sxs-lookup"><span data-stu-id="bb96c-126">-and-</span></span><br/><span data-ttu-id="bb96c-127">App tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="bb96c-127">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="bb96c-128">Observação: Isso se aplica ao pessoais contas da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="bb96c-128">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="bb96c-129">Inscrições criadas por **Este aplicativo** para o usuário entrou no apenas.</span><span class="sxs-lookup"><span data-stu-id="bb96c-129">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="bb96c-130">App está chamando em nome do próprio (permissão de aplicativo).</span><span class="sxs-lookup"><span data-stu-id="bb96c-130">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="bb96c-131">- e -</span><span class="sxs-lookup"><span data-stu-id="bb96c-131">-and-</span></span><br/><span data-ttu-id="bb96c-132">App tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="bb96c-132">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="bb96c-133">Observação: Isso se aplica a apenas contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="bb96c-133">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="bb96c-134">Inscrições criadas por **Este aplicativo** para si mesmo ou para qualquer usuário no diretório.</span><span class="sxs-lookup"><span data-stu-id="bb96c-134">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="bb96c-135">Cenários avançados</span><span class="sxs-lookup"><span data-stu-id="bb96c-135">Advanced scenarios</span></span>

<span data-ttu-id="bb96c-136">Em alguns casos, um aplicativo quer recuperar inscrições criadas por outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="bb96c-136">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="bb96c-137">Por exemplo, um usuário quiser ver todas as inscrições criadas por qualquer aplicativo em nome deles.</span><span class="sxs-lookup"><span data-stu-id="bb96c-137">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="bb96c-138">Ou então, um administrador talvez queira ver todas as inscrições de todos os aplicativos no seu diretório.</span><span class="sxs-lookup"><span data-stu-id="bb96c-138">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="bb96c-139">Para nesses cenários, uma permissão delegada Subscription.Read.All é necessária.</span><span class="sxs-lookup"><span data-stu-id="bb96c-139">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="bb96c-140">Contexto do aplicativo chamado</span><span class="sxs-lookup"><span data-stu-id="bb96c-140">Context of the calling app</span></span> | <span data-ttu-id="bb96c-141">Resposta conterá</span><span class="sxs-lookup"><span data-stu-id="bb96c-141">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="bb96c-142">App está chamando em nome do usuário conectado (delegada permissão).</span><span class="sxs-lookup"><span data-stu-id="bb96c-142">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="bb96c-143">*O usuário é um não seja o administrador*.</span><span class="sxs-lookup"><span data-stu-id="bb96c-143">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="bb96c-144">- e -</span><span class="sxs-lookup"><span data-stu-id="bb96c-144">-and-</span></span><br/><span data-ttu-id="bb96c-145">App tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb96c-145">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="bb96c-146">Observação: Isso se aplica ao pessoais contas da Microsoft e contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="bb96c-146">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="bb96c-147">Inscrições criadas por **qualquer aplicativo** para o usuário entrou no apenas.</span><span class="sxs-lookup"><span data-stu-id="bb96c-147">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="bb96c-148">App está chamando em nome do usuário conectado (delegada permissão).</span><span class="sxs-lookup"><span data-stu-id="bb96c-148">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="bb96c-149">*O usuário é um administrador*.</span><span class="sxs-lookup"><span data-stu-id="bb96c-149">*The user is an admin*.</span></span><br/><span data-ttu-id="bb96c-150">- e -</span><span class="sxs-lookup"><span data-stu-id="bb96c-150">-and-</span></span><br/><span data-ttu-id="bb96c-151">App tem a permissão Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb96c-151">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="bb96c-152">Observação: Isso se aplica a apenas contas de trabalho/escola.</span><span class="sxs-lookup"><span data-stu-id="bb96c-152">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="bb96c-153">Inscrições criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.</span><span class="sxs-lookup"><span data-stu-id="bb96c-153">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb96c-154">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb96c-154">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb96c-155">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bb96c-155">Optional query parameters</span></span>

<span data-ttu-id="bb96c-156">Este método não oferece suporte para os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bb96c-156">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb96c-157">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb96c-157">Request headers</span></span>

| <span data-ttu-id="bb96c-158">Nome</span><span class="sxs-lookup"><span data-stu-id="bb96c-158">Name</span></span>       | <span data-ttu-id="bb96c-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb96c-159">Type</span></span> | <span data-ttu-id="bb96c-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb96c-160">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bb96c-161">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb96c-161">Authorization</span></span>  | <span data-ttu-id="bb96c-162">string</span><span class="sxs-lookup"><span data-stu-id="bb96c-162">string</span></span>  | <span data-ttu-id="bb96c-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb96c-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb96c-165">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb96c-165">Request body</span></span>

<span data-ttu-id="bb96c-166">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb96c-166">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb96c-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb96c-167">Response</span></span>

<span data-ttu-id="bb96c-168">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos de [inscrição](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb96c-168">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb96c-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb96c-169">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bb96c-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb96c-170">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="bb96c-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb96c-171">Response</span></span>

<span data-ttu-id="bb96c-172">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb96c-172">Here is an example of the response.</span></span> <span data-ttu-id="bb96c-173">Observação: A resposta mostrada aqui pode estar truncada para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="bb96c-173">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="bb96c-174">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb96c-174">All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

<span data-ttu-id="bb96c-175">Quando uma solicitação retorna várias páginas de dados, a resposta inclui um `@odata.nextLink` propriedade para ajudá-lo a gerenciar os resultados.</span><span class="sxs-lookup"><span data-stu-id="bb96c-175">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="bb96c-176">Para saber mais, consulte [os dados de paginação Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="bb96c-176">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
