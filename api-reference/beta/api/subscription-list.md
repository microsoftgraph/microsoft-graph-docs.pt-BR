---
title: Listar de assinaturas
description: " Veja os cenários abaixo para obter detalhes."
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 3ffcf78c7df28faba22b92a7389f473f0ea91613
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335808"
---
# <a name="list-subscriptions"></a><span data-ttu-id="66129-103">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="66129-103">List subscriptions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66129-104">Recupere uma lista de assinaturas de webhook.</span><span class="sxs-lookup"><span data-stu-id="66129-104">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="66129-105">O conteúdo da resposta depende do contexto no qual o aplicativo está chamando; Veja os cenários abaixo para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="66129-105">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="66129-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="66129-106">Permissions</span></span>

<span data-ttu-id="66129-107">Essa API suporta os seguintes escopos de permissão; para saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66129-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66129-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66129-108">Permission type</span></span>  | <span data-ttu-id="66129-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66129-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="66129-110">[Delegado](/graph/auth-v2-user) (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66129-110">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="66129-111">Permissão necessária para [criar assinatura](subscription-post-subscriptions.md) ou assinatura. Read. All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="66129-111">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="66129-112">[Delegado](/graph/auth-v2-user) (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66129-112">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="66129-113">Permissão necessária para [criar assinatura](subscription-post-subscriptions.md) ou assinatura. Read. All (veja abaixo).</span><span class="sxs-lookup"><span data-stu-id="66129-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="66129-114">Application</span><span class="sxs-lookup"><span data-stu-id="66129-114">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="66129-115">Permissão necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="66129-115">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="66129-116">Os resultados da resposta são baseados no contexto do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="66129-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="66129-117">Veja a seguir um resumo dos cenários comuns:</span><span class="sxs-lookup"><span data-stu-id="66129-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="66129-118">Cenários básicos</span><span class="sxs-lookup"><span data-stu-id="66129-118">Basic scenarios</span></span>

<span data-ttu-id="66129-119">Normalmente, um aplicativo deseja recuperar as assinaturas criadas originalmente para o usuário conectado no momento ou para todos os usuários no diretório (contas corporativas/de estudante).</span><span class="sxs-lookup"><span data-stu-id="66129-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="66129-120">Esses cenários não exigem nenhuma permissão especial além daquelas que o aplicativo usava originalmente para criar suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="66129-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="66129-121">Contexto do aplicativo de chamada</span><span class="sxs-lookup"><span data-stu-id="66129-121">Context of the calling app</span></span> | <span data-ttu-id="66129-122">Resposta contém</span><span class="sxs-lookup"><span data-stu-id="66129-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="66129-123">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="66129-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="66129-124">e</span><span class="sxs-lookup"><span data-stu-id="66129-124">-and-</span></span><br/><span data-ttu-id="66129-125">O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="66129-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="66129-126">Observação: isso se aplica às contas da Microsoft pessoais e às contas corporativas/de estudante.</span><span class="sxs-lookup"><span data-stu-id="66129-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="66129-127">Assinaturas criadas por **este aplicativo** somente para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="66129-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="66129-128">O aplicativo está chamando em nome de si mesmo (permissão de aplicativo).</span><span class="sxs-lookup"><span data-stu-id="66129-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="66129-129">e</span><span class="sxs-lookup"><span data-stu-id="66129-129">-and-</span></span><br/><span data-ttu-id="66129-130">O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="66129-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="66129-131">Observação: isso se aplica apenas às contas corporativas/de estudante.</span><span class="sxs-lookup"><span data-stu-id="66129-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="66129-132">Assinaturas criadas por **este aplicativo** para si mesmo ou para qualquer usuário no diretório.</span><span class="sxs-lookup"><span data-stu-id="66129-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="66129-133">Cenários avançados</span><span class="sxs-lookup"><span data-stu-id="66129-133">Advanced scenarios</span></span>

<span data-ttu-id="66129-134">Em alguns casos, um aplicativo deseja recuperar assinaturas criadas por outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="66129-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="66129-135">Por exemplo, um usuário deseja ver todas as assinaturas criadas por qualquer aplicativo em seu nome.</span><span class="sxs-lookup"><span data-stu-id="66129-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="66129-136">Ou, um administrador pode querer ver todas as assinaturas de todos os aplicativos em seu diretório.</span><span class="sxs-lookup"><span data-stu-id="66129-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="66129-137">Para esses cenários, uma assinatura de permissão delegada. Read. All é necessário.</span><span class="sxs-lookup"><span data-stu-id="66129-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="66129-138">Contexto do aplicativo de chamada</span><span class="sxs-lookup"><span data-stu-id="66129-138">Context of the calling app</span></span> | <span data-ttu-id="66129-139">Resposta contém</span><span class="sxs-lookup"><span data-stu-id="66129-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="66129-140">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="66129-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="66129-141">*O usuário não é um administrador*.</span><span class="sxs-lookup"><span data-stu-id="66129-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="66129-142">e</span><span class="sxs-lookup"><span data-stu-id="66129-142">-and-</span></span><br/><span data-ttu-id="66129-143">O aplicativo tem a permissão Subscription. Read. All</span><span class="sxs-lookup"><span data-stu-id="66129-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="66129-144">Observação: isso se aplica às contas da Microsoft pessoais e às contas corporativas/de estudante.</span><span class="sxs-lookup"><span data-stu-id="66129-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="66129-145">Assinaturas criadas por **qualquer aplicativo** somente para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="66129-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="66129-146">O aplicativo está chamando em nome do usuário conectado (permissão delegada).</span><span class="sxs-lookup"><span data-stu-id="66129-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="66129-147">*O usuário é um administrador*.</span><span class="sxs-lookup"><span data-stu-id="66129-147">*The user is an admin*.</span></span><br/><span data-ttu-id="66129-148">e</span><span class="sxs-lookup"><span data-stu-id="66129-148">-and-</span></span><br/><span data-ttu-id="66129-149">O aplicativo tem a permissão Subscription. Read. All</span><span class="sxs-lookup"><span data-stu-id="66129-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="66129-150">Observação: isso se aplica apenas às contas corporativas/de estudante.</span><span class="sxs-lookup"><span data-stu-id="66129-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="66129-151">Assinaturas criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.</span><span class="sxs-lookup"><span data-stu-id="66129-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66129-152">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66129-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66129-153">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="66129-153">Optional query parameters</span></span>

<span data-ttu-id="66129-154">Este método não oferece suporte aos [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="66129-154">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66129-155">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66129-155">Request headers</span></span>

| <span data-ttu-id="66129-156">Nome</span><span class="sxs-lookup"><span data-stu-id="66129-156">Name</span></span>       | <span data-ttu-id="66129-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="66129-157">Type</span></span> | <span data-ttu-id="66129-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="66129-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66129-159">Autorização</span><span class="sxs-lookup"><span data-stu-id="66129-159">Authorization</span></span>  | <span data-ttu-id="66129-160">string</span><span class="sxs-lookup"><span data-stu-id="66129-160">string</span></span>  | <span data-ttu-id="66129-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66129-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66129-163">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66129-163">Request body</span></span>

<span data-ttu-id="66129-164">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66129-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66129-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="66129-165">Response</span></span>

<span data-ttu-id="66129-166">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de objetos [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66129-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66129-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66129-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="66129-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66129-168">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="66129-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="66129-169">Response</span></span>

<span data-ttu-id="66129-170">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66129-170">Here is an example of the response.</span></span> <span data-ttu-id="66129-171">Observação: a resposta mostrada aqui pode ser truncada por brevidade.</span><span class="sxs-lookup"><span data-stu-id="66129-171">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="66129-172">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66129-172">All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->

<span data-ttu-id="66129-173">Quando uma solicitação retorna várias páginas de dados, a resposta inclui uma `@odata.nextLink` propriedade para ajudá-lo a gerenciar os resultados.</span><span class="sxs-lookup"><span data-stu-id="66129-173">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="66129-174">Para saber mais, confira paGinação [de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="66129-174">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
