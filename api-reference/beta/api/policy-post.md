---
title: Criar política
description: Crie um novo objeto de diretiva especificando o nome para exibição, tipo de política e descrição da política.
ms.openlocfilehash: fca6201d7afa6a78f15da0d37fb611e4114783e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040277"
---
# <a name="create-policy"></a><span data-ttu-id="069a0-103">Criar política</span><span class="sxs-lookup"><span data-stu-id="069a0-103">Create Policy</span></span>

> <span data-ttu-id="069a0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="069a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="069a0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="069a0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="069a0-106">Crie um novo objeto de [diretiva](../resources/policy.md) especificando o nome para exibição, tipo de política e descrição da política.</span><span class="sxs-lookup"><span data-stu-id="069a0-106">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="069a0-107">Observação: Os detalhes da diretiva serão validados antes de serem armazenados.</span><span class="sxs-lookup"><span data-stu-id="069a0-107">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="069a0-108">Se ele não passar na validação, um 400 Solicitação incorreta será retornado.</span><span class="sxs-lookup"><span data-stu-id="069a0-108">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="069a0-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="069a0-109">Permissions</span></span>
<span data-ttu-id="069a0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="069a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="069a0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="069a0-112">Permission type</span></span>      | <span data-ttu-id="069a0-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="069a0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="069a0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="069a0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="069a0-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="069a0-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="069a0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="069a0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="069a0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="069a0-117">Not supported.</span></span>    |
|<span data-ttu-id="069a0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="069a0-118">Application</span></span> | <span data-ttu-id="069a0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="069a0-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="069a0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="069a0-120">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="069a0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="069a0-121">Request headers</span></span>
| <span data-ttu-id="069a0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="069a0-122">Name</span></span>       | <span data-ttu-id="069a0-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="069a0-123">Type</span></span> | <span data-ttu-id="069a0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="069a0-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="069a0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="069a0-125">Authorization</span></span>  | <span data-ttu-id="069a0-126">string</span><span class="sxs-lookup"><span data-stu-id="069a0-126">string</span></span>  | <span data-ttu-id="069a0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="069a0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="069a0-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="069a0-129">Content-Type</span></span> | <span data-ttu-id="069a0-130">application/json</span><span class="sxs-lookup"><span data-stu-id="069a0-130">application/json</span></span>  | <span data-ttu-id="069a0-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="069a0-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="069a0-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="069a0-133">Request body</span></span>
<span data-ttu-id="069a0-134">No corpo da solicitação, fornecem uma representação de JSON do objeto de [diretiva](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="069a0-134">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="069a0-135">A tabela a seguir mostra as propriedades que são necessárias quando você criar uma diretiva.</span><span class="sxs-lookup"><span data-stu-id="069a0-135">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="069a0-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="069a0-136">Parameter</span></span>    | <span data-ttu-id="069a0-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="069a0-137">Type</span></span>   |<span data-ttu-id="069a0-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="069a0-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="069a0-139">definição</span><span class="sxs-lookup"><span data-stu-id="069a0-139">definition</span></span>|<span data-ttu-id="069a0-140">String</span><span class="sxs-lookup"><span data-stu-id="069a0-140">String</span></span>|<span data-ttu-id="069a0-141">A versão de cadeia de caracteres do objeto de [diretiva](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="069a0-141">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="069a0-142">displayName</span><span class="sxs-lookup"><span data-stu-id="069a0-142">displayName</span></span>|<span data-ttu-id="069a0-143">String</span><span class="sxs-lookup"><span data-stu-id="069a0-143">String</span></span>|<span data-ttu-id="069a0-144">Um nome personalizado para a política.</span><span class="sxs-lookup"><span data-stu-id="069a0-144">A custom name for the policy.</span></span>|
|<span data-ttu-id="069a0-145">type</span><span class="sxs-lookup"><span data-stu-id="069a0-145">type</span></span>|<span data-ttu-id="069a0-146">String</span><span class="sxs-lookup"><span data-stu-id="069a0-146">String</span></span>|<span data-ttu-id="069a0-147">Especifica o tipo de política.</span><span class="sxs-lookup"><span data-stu-id="069a0-147">Specifies the type of policy.</span></span> <span data-ttu-id="069a0-148">No momento deve ser "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="069a0-148">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="069a0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="069a0-149">Response</span></span>

<span data-ttu-id="069a0-150">Se tiver êxito, este método retornará `201 Created` objeto de código e a [diretiva](../resources/policy.md) de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="069a0-150">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="069a0-151">Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="069a0-151">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="069a0-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="069a0-152">Example</span></span>
<span data-ttu-id="069a0-153">O exemplo a seguir cria uma nova vida útil do token política.</span><span class="sxs-lookup"><span data-stu-id="069a0-153">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="069a0-154">Observe que o parâmetro de definição de cadeia de caracteres tem escape aspas duplas.</span><span class="sxs-lookup"><span data-stu-id="069a0-154">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="069a0-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="069a0-155">Request</span></span>
<span data-ttu-id="069a0-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="069a0-156">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="069a0-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="069a0-157">Response</span></span>
<span data-ttu-id="069a0-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="069a0-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
