---
title: Criar política
description: Criar um novo objeto de política especificando o nome de exibição, o tipo de política e a descrição da política.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2e13ef2bdcf424d68d94d97412487708022386cb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455498"
---
# <a name="create-policy"></a><span data-ttu-id="a210c-103">Criar política</span><span class="sxs-lookup"><span data-stu-id="a210c-103">Create Policy</span></span>

<span data-ttu-id="a210c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a210c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a210c-105">Criar um novo objeto de [política](../resources/policy.md) especificando o nome de exibição, o tipo de política e a descrição da política.</span><span class="sxs-lookup"><span data-stu-id="a210c-105">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="a210c-106">Observação: os detalhes da política serão validados antes de serem armazenados.</span><span class="sxs-lookup"><span data-stu-id="a210c-106">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="a210c-107">Se ele não passar na validação, uma solicitação inválida 400 será retornada.</span><span class="sxs-lookup"><span data-stu-id="a210c-107">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="a210c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a210c-108">Permissions</span></span>
<span data-ttu-id="a210c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a210c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a210c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a210c-111">Permission type</span></span>      | <span data-ttu-id="a210c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a210c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a210c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a210c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a210c-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a210c-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a210c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a210c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a210c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a210c-116">Not supported.</span></span>    |
|<span data-ttu-id="a210c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a210c-117">Application</span></span> | <span data-ttu-id="a210c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a210c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a210c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a210c-119">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="a210c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a210c-120">Request headers</span></span>
| <span data-ttu-id="a210c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a210c-121">Name</span></span>       | <span data-ttu-id="a210c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a210c-122">Type</span></span> | <span data-ttu-id="a210c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a210c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a210c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a210c-124">Authorization</span></span>  | <span data-ttu-id="a210c-125">string</span><span class="sxs-lookup"><span data-stu-id="a210c-125">string</span></span>  | <span data-ttu-id="a210c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a210c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a210c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a210c-128">Content-Type</span></span> | <span data-ttu-id="a210c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a210c-129">application/json</span></span>  | <span data-ttu-id="a210c-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a210c-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a210c-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a210c-132">Request body</span></span>
<span data-ttu-id="a210c-133">No corpo da solicitação, forneça uma representação JSON do objeto [Policy](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="a210c-133">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="a210c-134">A tabela a seguir mostra as propriedades que são necessárias ao criar uma política.</span><span class="sxs-lookup"><span data-stu-id="a210c-134">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="a210c-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a210c-135">Parameter</span></span>    | <span data-ttu-id="a210c-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="a210c-136">Type</span></span>   |<span data-ttu-id="a210c-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="a210c-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a210c-138">definir</span><span class="sxs-lookup"><span data-stu-id="a210c-138">definition</span></span>|<span data-ttu-id="a210c-139">String</span><span class="sxs-lookup"><span data-stu-id="a210c-139">String</span></span>|<span data-ttu-id="a210c-140">A versão de cadeia de caracteres do objeto [Policy](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="a210c-140">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="a210c-141">displayName</span><span class="sxs-lookup"><span data-stu-id="a210c-141">displayName</span></span>|<span data-ttu-id="a210c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a210c-142">String</span></span>|<span data-ttu-id="a210c-143">Um nome personalizado para a política.</span><span class="sxs-lookup"><span data-stu-id="a210c-143">A custom name for the policy.</span></span>|
|<span data-ttu-id="a210c-144">type</span><span class="sxs-lookup"><span data-stu-id="a210c-144">type</span></span>|<span data-ttu-id="a210c-145">String</span><span class="sxs-lookup"><span data-stu-id="a210c-145">String</span></span>|<span data-ttu-id="a210c-146">Especifica o tipo de política.</span><span class="sxs-lookup"><span data-stu-id="a210c-146">Specifies the type of policy.</span></span> <span data-ttu-id="a210c-147">No momento, deve ser "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="a210c-147">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="a210c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a210c-148">Response</span></span>

<span data-ttu-id="a210c-149">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Policy](../resources/policy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a210c-149">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="a210c-150">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="a210c-150">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="a210c-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a210c-151">Example</span></span>
<span data-ttu-id="a210c-152">O exemplo a seguir cria uma nova política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="a210c-152">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="a210c-153">Observe que o parâmetro de definição de cadeia de caracteres tem aspas duplas de escape.</span><span class="sxs-lookup"><span data-stu-id="a210c-153">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="a210c-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a210c-154">Request</span></span>
<span data-ttu-id="a210c-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a210c-155">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="a210c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a210c-156">Response</span></span>
<span data-ttu-id="a210c-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a210c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
  "id":"id-value",
  "alternativeIdentifier":null,
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "displayName":"name-value",
  "isOrganizationDefault":false,
  "keyCredentials",
  "type":"TokenLifetimePolicy"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
