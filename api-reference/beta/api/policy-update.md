---
title: Política de atualização
description: Atualize as propriedades em uma política preexistente.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 81c9d429ba3a74d854a9d091f6e40af7993916f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455489"
---
# <a name="update-policy"></a><span data-ttu-id="f8b7a-103">Política de atualização</span><span class="sxs-lookup"><span data-stu-id="f8b7a-103">Update Policy</span></span>

<span data-ttu-id="f8b7a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f8b7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8b7a-105">Atualize as propriedades em uma [política](../resources/policy.md)preexistente.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-105">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8b7a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8b7a-106">Permissions</span></span>
<span data-ttu-id="f8b7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8b7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8b7a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8b7a-109">Permission type</span></span>      | <span data-ttu-id="f8b7a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8b7a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8b7a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8b7a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f8b7a-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f8b7a-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f8b7a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8b7a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8b7a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-114">Not supported.</span></span>    |
|<span data-ttu-id="f8b7a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8b7a-115">Application</span></span> | <span data-ttu-id="f8b7a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8b7a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8b7a-117">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f8b7a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8b7a-118">Request headers</span></span>
| <span data-ttu-id="f8b7a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f8b7a-119">Name</span></span>       | <span data-ttu-id="f8b7a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8b7a-120">Type</span></span> | <span data-ttu-id="f8b7a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8b7a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f8b7a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8b7a-122">Authorization</span></span>  | <span data-ttu-id="f8b7a-123">string</span><span class="sxs-lookup"><span data-stu-id="f8b7a-123">string</span></span>  | <span data-ttu-id="f8b7a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f8b7a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f8b7a-126">Content-Type</span></span> | <span data-ttu-id="f8b7a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f8b7a-127">application/json</span></span>  | <span data-ttu-id="f8b7a-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8b7a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8b7a-130">Request body</span></span>
<span data-ttu-id="f8b7a-131">No corpo da solicitação, forneça um objeto JSON com os parâmetros que precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-131">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="f8b7a-132">A tabela a seguir mostra os parâmetros possíveis.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-132">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="f8b7a-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f8b7a-133">Parameter</span></span>    | <span data-ttu-id="f8b7a-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8b7a-134">Type</span></span>   |<span data-ttu-id="f8b7a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8b7a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8b7a-136">definir</span><span class="sxs-lookup"><span data-stu-id="f8b7a-136">definition</span></span>|<span data-ttu-id="f8b7a-137">String</span><span class="sxs-lookup"><span data-stu-id="f8b7a-137">String</span></span>|<span data-ttu-id="f8b7a-138">A versão do em formato do objeto [Policy](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="f8b7a-138">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="f8b7a-139">displayName</span><span class="sxs-lookup"><span data-stu-id="f8b7a-139">displayName</span></span>|<span data-ttu-id="f8b7a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8b7a-140">String</span></span>|<span data-ttu-id="f8b7a-141">Um nome personalizado para a política.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-141">A custom name for the policy.</span></span>|
|<span data-ttu-id="f8b7a-142">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="f8b7a-142">isOrganizationDefault</span></span>|<span data-ttu-id="f8b7a-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b7a-143">Boolean</span></span>|<span data-ttu-id="f8b7a-144">Especifica se essa política é aplicada por padrão.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-144">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="f8b7a-145">type</span><span class="sxs-lookup"><span data-stu-id="f8b7a-145">type</span></span>|<span data-ttu-id="f8b7a-146">String</span><span class="sxs-lookup"><span data-stu-id="f8b7a-146">String</span></span>|<span data-ttu-id="f8b7a-147">Especifica o tipo de política.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-147">Specifies the type of policy.</span></span> <span data-ttu-id="f8b7a-148">No momento, deve ser "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="f8b7a-148">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="f8b7a-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8b7a-149">Response</span></span>

<span data-ttu-id="f8b7a-150">Quando é bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-150">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="f8b7a-151">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-151">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="f8b7a-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8b7a-152">Example</span></span>
<span data-ttu-id="f8b7a-153">O exemplo a seguir atualiza a definição da política de tempo de vida do token e define-a como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-153">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="f8b7a-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8b7a-154">Request</span></span>
<span data-ttu-id="f8b7a-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-155">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="f8b7a-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8b7a-156">Response</span></span>
<span data-ttu-id="f8b7a-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8b7a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
