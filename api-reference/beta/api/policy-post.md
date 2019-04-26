---
title: Criar política
description: Criar um novo objeto de política especificando o nome de exibição, o tipo de política e a descrição da política.
localization_priority: Normal
ms.openlocfilehash: 4521f6fb032f936aec27cc5cac47d27e62bd2a3a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332186"
---
# <a name="create-policy"></a><span data-ttu-id="18878-103">Criar política</span><span class="sxs-lookup"><span data-stu-id="18878-103">Create Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18878-104">Criar um novo objeto de [política](../resources/policy.md) especificando o nome de exibição, o tipo de política e a descrição da política.</span><span class="sxs-lookup"><span data-stu-id="18878-104">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="18878-105">Observação: os detalhes da política serão validados antes de serem armazenados.</span><span class="sxs-lookup"><span data-stu-id="18878-105">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="18878-106">Se ele não passar na validação, uma solicitação inVálida 400 será retornada.</span><span class="sxs-lookup"><span data-stu-id="18878-106">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="18878-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="18878-107">Permissions</span></span>
<span data-ttu-id="18878-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18878-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18878-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18878-110">Permission type</span></span>      | <span data-ttu-id="18878-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18878-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18878-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18878-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18878-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18878-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="18878-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18878-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18878-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18878-115">Not supported.</span></span>    |
|<span data-ttu-id="18878-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18878-116">Application</span></span> | <span data-ttu-id="18878-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18878-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18878-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18878-118">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="18878-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18878-119">Request headers</span></span>
| <span data-ttu-id="18878-120">Nome</span><span class="sxs-lookup"><span data-stu-id="18878-120">Name</span></span>       | <span data-ttu-id="18878-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="18878-121">Type</span></span> | <span data-ttu-id="18878-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="18878-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18878-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18878-123">Authorization</span></span>  | <span data-ttu-id="18878-124">string</span><span class="sxs-lookup"><span data-stu-id="18878-124">string</span></span>  | <span data-ttu-id="18878-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18878-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18878-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18878-127">Content-Type</span></span> | <span data-ttu-id="18878-128">application/json</span><span class="sxs-lookup"><span data-stu-id="18878-128">application/json</span></span>  | <span data-ttu-id="18878-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18878-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18878-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18878-131">Request body</span></span>
<span data-ttu-id="18878-132">No corpo da solicitação, forneça uma representação JSON do objeto [Policy](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="18878-132">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="18878-133">A tabela a seguir mostra as propriedades que são necessárias ao criar uma política.</span><span class="sxs-lookup"><span data-stu-id="18878-133">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="18878-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="18878-134">Parameter</span></span>    | <span data-ttu-id="18878-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="18878-135">Type</span></span>   |<span data-ttu-id="18878-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="18878-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18878-137">definir</span><span class="sxs-lookup"><span data-stu-id="18878-137">definition</span></span>|<span data-ttu-id="18878-138">String</span><span class="sxs-lookup"><span data-stu-id="18878-138">String</span></span>|<span data-ttu-id="18878-139">A versão de cadeia de caracteres do objeto [Policy](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="18878-139">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="18878-140">displayName</span><span class="sxs-lookup"><span data-stu-id="18878-140">displayName</span></span>|<span data-ttu-id="18878-141">String</span><span class="sxs-lookup"><span data-stu-id="18878-141">String</span></span>|<span data-ttu-id="18878-142">Um nome personalizado para a política.</span><span class="sxs-lookup"><span data-stu-id="18878-142">A custom name for the policy.</span></span>|
|<span data-ttu-id="18878-143">tipo</span><span class="sxs-lookup"><span data-stu-id="18878-143">type</span></span>|<span data-ttu-id="18878-144">String</span><span class="sxs-lookup"><span data-stu-id="18878-144">String</span></span>|<span data-ttu-id="18878-145">Especifica o tipo de política.</span><span class="sxs-lookup"><span data-stu-id="18878-145">Specifies the type of policy.</span></span> <span data-ttu-id="18878-146">No momento, deve ser "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="18878-146">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="18878-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="18878-147">Response</span></span>

<span data-ttu-id="18878-148">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Policy](../resources/policy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18878-148">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="18878-149">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="18878-149">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="18878-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18878-150">Example</span></span>
<span data-ttu-id="18878-151">O exemplo a seguir cria uma nova política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="18878-151">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="18878-152">Observe que o parâmetro de definição de cadeia de caracteres tem aspas duplas de escape.</span><span class="sxs-lookup"><span data-stu-id="18878-152">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="18878-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18878-153">Request</span></span>
<span data-ttu-id="18878-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18878-154">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="18878-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="18878-155">Response</span></span>
<span data-ttu-id="18878-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18878-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
