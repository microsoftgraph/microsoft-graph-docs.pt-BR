---
title: Política de atualização
description: Atualize propriedades em uma diretiva preexistente.
localization_priority: Normal
ms.openlocfilehash: 2992f2f76c0e8b213ad8aabca1bfd0fe59883989
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857152"
---
# <a name="update-policy"></a><span data-ttu-id="7f9de-103">Política de atualização</span><span class="sxs-lookup"><span data-stu-id="7f9de-103">Update Policy</span></span>

> <span data-ttu-id="7f9de-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7f9de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f9de-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7f9de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f9de-106">Atualize propriedades em uma [política](../resources/policy.md)de preexistente.</span><span class="sxs-lookup"><span data-stu-id="7f9de-106">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f9de-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="7f9de-107">Permissions</span></span>
<span data-ttu-id="7f9de-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f9de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f9de-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f9de-110">Permission type</span></span>      | <span data-ttu-id="7f9de-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f9de-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f9de-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f9de-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7f9de-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7f9de-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7f9de-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f9de-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f9de-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f9de-115">Not supported.</span></span>    |
|<span data-ttu-id="7f9de-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f9de-116">Application</span></span> | <span data-ttu-id="7f9de-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f9de-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f9de-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f9de-118">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7f9de-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9de-119">Request headers</span></span>
| <span data-ttu-id="7f9de-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7f9de-120">Name</span></span>       | <span data-ttu-id="7f9de-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f9de-121">Type</span></span> | <span data-ttu-id="7f9de-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f9de-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7f9de-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f9de-123">Authorization</span></span>  | <span data-ttu-id="7f9de-124">string</span><span class="sxs-lookup"><span data-stu-id="7f9de-124">string</span></span>  | <span data-ttu-id="7f9de-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f9de-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f9de-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f9de-127">Content-Type</span></span> | <span data-ttu-id="7f9de-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7f9de-128">application/json</span></span>  | <span data-ttu-id="7f9de-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f9de-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f9de-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9de-131">Request body</span></span>
<span data-ttu-id="7f9de-132">No corpo da solicitação, fornecem um objeto JSON com os parâmetros que precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="7f9de-132">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="7f9de-133">A tabela a seguir mostra os parâmetros possíveis.</span><span class="sxs-lookup"><span data-stu-id="7f9de-133">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="7f9de-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7f9de-134">Parameter</span></span>    | <span data-ttu-id="7f9de-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f9de-135">Type</span></span>   |<span data-ttu-id="7f9de-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f9de-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f9de-137">definição</span><span class="sxs-lookup"><span data-stu-id="7f9de-137">definition</span></span>|<span data-ttu-id="7f9de-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f9de-138">String</span></span>|<span data-ttu-id="7f9de-139">A versão stringified do objeto de [diretiva](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="7f9de-139">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="7f9de-140">displayName</span><span class="sxs-lookup"><span data-stu-id="7f9de-140">displayName</span></span>|<span data-ttu-id="7f9de-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f9de-141">String</span></span>|<span data-ttu-id="7f9de-142">Um nome personalizado para a política.</span><span class="sxs-lookup"><span data-stu-id="7f9de-142">A custom name for the policy.</span></span>|
|<span data-ttu-id="7f9de-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="7f9de-143">isOrganizationDefault</span></span>|<span data-ttu-id="7f9de-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="7f9de-144">Boolean</span></span>|<span data-ttu-id="7f9de-145">Especifica se esta política é aplicada por padrão.</span><span class="sxs-lookup"><span data-stu-id="7f9de-145">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="7f9de-146">type</span><span class="sxs-lookup"><span data-stu-id="7f9de-146">type</span></span>|<span data-ttu-id="7f9de-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f9de-147">String</span></span>|<span data-ttu-id="7f9de-148">Especifica o tipo de política.</span><span class="sxs-lookup"><span data-stu-id="7f9de-148">Specifies the type of policy.</span></span> <span data-ttu-id="7f9de-149">No momento deve ser "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="7f9de-149">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="7f9de-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9de-150">Response</span></span>

<span data-ttu-id="7f9de-151">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7f9de-151">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="7f9de-152">Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="7f9de-152">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="7f9de-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f9de-153">Example</span></span>
<span data-ttu-id="7f9de-154">O exemplo a seguir atualiza a definição da diretiva de vida útil do token e define como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="7f9de-154">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="7f9de-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9de-155">Request</span></span>
<span data-ttu-id="7f9de-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f9de-156">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="7f9de-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9de-157">Response</span></span>
<span data-ttu-id="7f9de-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f9de-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
