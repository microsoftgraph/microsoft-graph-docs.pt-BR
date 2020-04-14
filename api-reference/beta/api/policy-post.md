---
title: Criar política
description: Criar um novo objeto de política especificando o nome de exibição, o tipo de política e a descrição da política.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: 04bc6134529b4d7192ed50a849fc487970f6b812
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408306"
---
# <a name="create-policy"></a><span data-ttu-id="97e49-103">Criar política</span><span class="sxs-lookup"><span data-stu-id="97e49-103">Create Policy</span></span>

<span data-ttu-id="97e49-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97e49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97e49-105">Criar um novo objeto de [política](../resources/policy.md) especificando o nome de exibição, o tipo de política e a descrição da política.</span><span class="sxs-lookup"><span data-stu-id="97e49-105">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="97e49-106">Observação: os detalhes da política serão validados antes de serem armazenados.</span><span class="sxs-lookup"><span data-stu-id="97e49-106">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="97e49-107">Se ele não passar na validação, uma solicitação inválida 400 será retornada.</span><span class="sxs-lookup"><span data-stu-id="97e49-107">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="97e49-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="97e49-108">Permissions</span></span>
<span data-ttu-id="97e49-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97e49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97e49-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97e49-111">Permission type</span></span>      | <span data-ttu-id="97e49-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97e49-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97e49-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97e49-113">Delegated (work or school account)</span></span> | <span data-ttu-id="97e49-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="97e49-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="97e49-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97e49-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97e49-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97e49-116">Not supported.</span></span>    |
|<span data-ttu-id="97e49-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97e49-117">Application</span></span> | <span data-ttu-id="97e49-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97e49-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97e49-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97e49-119">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="97e49-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97e49-120">Request headers</span></span>
| <span data-ttu-id="97e49-121">Nome</span><span class="sxs-lookup"><span data-stu-id="97e49-121">Name</span></span>       | <span data-ttu-id="97e49-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="97e49-122">Type</span></span> | <span data-ttu-id="97e49-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="97e49-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="97e49-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="97e49-124">Authorization</span></span>  | <span data-ttu-id="97e49-125">string</span><span class="sxs-lookup"><span data-stu-id="97e49-125">string</span></span>  | <span data-ttu-id="97e49-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97e49-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97e49-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97e49-128">Content-Type</span></span> | <span data-ttu-id="97e49-129">application/json</span><span class="sxs-lookup"><span data-stu-id="97e49-129">application/json</span></span>  | <span data-ttu-id="97e49-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97e49-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97e49-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97e49-132">Request body</span></span>
<span data-ttu-id="97e49-133">No corpo da solicitação, forneça uma representação JSON do objeto [Policy](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="97e49-133">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="97e49-134">A tabela a seguir mostra as propriedades que são necessárias ao criar uma política.</span><span class="sxs-lookup"><span data-stu-id="97e49-134">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="97e49-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="97e49-135">Parameter</span></span>    | <span data-ttu-id="97e49-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="97e49-136">Type</span></span>   |<span data-ttu-id="97e49-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="97e49-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97e49-138">definir</span><span class="sxs-lookup"><span data-stu-id="97e49-138">definition</span></span>|<span data-ttu-id="97e49-139">String</span><span class="sxs-lookup"><span data-stu-id="97e49-139">String</span></span>|<span data-ttu-id="97e49-140">A versão de cadeia de caracteres do objeto [Policy](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="97e49-140">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="97e49-141">displayName</span><span class="sxs-lookup"><span data-stu-id="97e49-141">displayName</span></span>|<span data-ttu-id="97e49-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97e49-142">String</span></span>|<span data-ttu-id="97e49-143">Um nome personalizado para a política.</span><span class="sxs-lookup"><span data-stu-id="97e49-143">A custom name for the policy.</span></span>|
|<span data-ttu-id="97e49-144">type</span><span class="sxs-lookup"><span data-stu-id="97e49-144">type</span></span>|<span data-ttu-id="97e49-145">String</span><span class="sxs-lookup"><span data-stu-id="97e49-145">String</span></span>|<span data-ttu-id="97e49-146">Especifica o tipo de política.</span><span class="sxs-lookup"><span data-stu-id="97e49-146">Specifies the type of policy.</span></span> <span data-ttu-id="97e49-147">No momento, deve ser "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="97e49-147">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="97e49-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="97e49-148">Response</span></span>

<span data-ttu-id="97e49-149">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Policy](../resources/policy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97e49-149">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="97e49-150">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="97e49-150">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="97e49-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97e49-151">Example</span></span>
<span data-ttu-id="97e49-152">O exemplo a seguir cria uma nova política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="97e49-152">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="97e49-153">Observe que o parâmetro de definição de cadeia de caracteres tem aspas duplas de escape.</span><span class="sxs-lookup"><span data-stu-id="97e49-153">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="97e49-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97e49-154">Request</span></span>
<span data-ttu-id="97e49-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97e49-155">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="97e49-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="97e49-156">Response</span></span>
<span data-ttu-id="97e49-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97e49-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
