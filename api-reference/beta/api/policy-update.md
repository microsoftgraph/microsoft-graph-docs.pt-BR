---
title: Política de atualização
description: Atualize propriedades em uma diretiva preexistente.
localization_priority: Normal
ms.openlocfilehash: d99aa42c4a67f6b874cbc1e266da76287388c05e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515409"
---
# <a name="update-policy"></a><span data-ttu-id="d19f1-103">Política de atualização</span><span class="sxs-lookup"><span data-stu-id="d19f1-103">Update Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d19f1-104">Atualize propriedades em uma [política](../resources/policy.md)de preexistente.</span><span class="sxs-lookup"><span data-stu-id="d19f1-104">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d19f1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d19f1-105">Permissions</span></span>
<span data-ttu-id="d19f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d19f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d19f1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d19f1-108">Permission type</span></span>      | <span data-ttu-id="d19f1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d19f1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d19f1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d19f1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d19f1-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d19f1-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d19f1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d19f1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d19f1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d19f1-113">Not supported.</span></span>    |
|<span data-ttu-id="d19f1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d19f1-114">Application</span></span> | <span data-ttu-id="d19f1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d19f1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d19f1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d19f1-116">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d19f1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d19f1-117">Request headers</span></span>
| <span data-ttu-id="d19f1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d19f1-118">Name</span></span>       | <span data-ttu-id="d19f1-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d19f1-119">Type</span></span> | <span data-ttu-id="d19f1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d19f1-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d19f1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d19f1-121">Authorization</span></span>  | <span data-ttu-id="d19f1-122">string</span><span class="sxs-lookup"><span data-stu-id="d19f1-122">string</span></span>  | <span data-ttu-id="d19f1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d19f1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d19f1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d19f1-125">Content-Type</span></span> | <span data-ttu-id="d19f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d19f1-126">application/json</span></span>  | <span data-ttu-id="d19f1-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d19f1-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d19f1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d19f1-129">Request body</span></span>
<span data-ttu-id="d19f1-130">No corpo da solicitação, fornecem um objeto JSON com os parâmetros que precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d19f1-130">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="d19f1-131">A tabela a seguir mostra os parâmetros possíveis.</span><span class="sxs-lookup"><span data-stu-id="d19f1-131">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="d19f1-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d19f1-132">Parameter</span></span>    | <span data-ttu-id="d19f1-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="d19f1-133">Type</span></span>   |<span data-ttu-id="d19f1-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d19f1-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d19f1-135">Definição</span><span class="sxs-lookup"><span data-stu-id="d19f1-135">definition</span></span>|<span data-ttu-id="d19f1-136">String</span><span class="sxs-lookup"><span data-stu-id="d19f1-136">String</span></span>|<span data-ttu-id="d19f1-137">A versão stringified do objeto de [diretiva](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="d19f1-137">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="d19f1-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d19f1-138">displayName</span></span>|<span data-ttu-id="d19f1-139">String</span><span class="sxs-lookup"><span data-stu-id="d19f1-139">String</span></span>|<span data-ttu-id="d19f1-140">Um nome personalizado para a política.</span><span class="sxs-lookup"><span data-stu-id="d19f1-140">A custom name for the policy.</span></span>|
|<span data-ttu-id="d19f1-141">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="d19f1-141">isOrganizationDefault</span></span>|<span data-ttu-id="d19f1-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="d19f1-142">Boolean</span></span>|<span data-ttu-id="d19f1-143">Especifica se esta política é aplicada por padrão.</span><span class="sxs-lookup"><span data-stu-id="d19f1-143">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="d19f1-144">type</span><span class="sxs-lookup"><span data-stu-id="d19f1-144">type</span></span>|<span data-ttu-id="d19f1-145">String</span><span class="sxs-lookup"><span data-stu-id="d19f1-145">String</span></span>|<span data-ttu-id="d19f1-146">Especifica o tipo de política.</span><span class="sxs-lookup"><span data-stu-id="d19f1-146">Specifies the type of policy.</span></span> <span data-ttu-id="d19f1-147">No momento deve ser "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="d19f1-147">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="d19f1-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d19f1-148">Response</span></span>

<span data-ttu-id="d19f1-149">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d19f1-149">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="d19f1-150">Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="d19f1-150">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="d19f1-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d19f1-151">Example</span></span>
<span data-ttu-id="d19f1-152">O exemplo a seguir atualiza a definição da diretiva de vida útil do token e define como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="d19f1-152">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="d19f1-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d19f1-153">Request</span></span>
<span data-ttu-id="d19f1-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d19f1-154">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="d19f1-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="d19f1-155">Response</span></span>
<span data-ttu-id="d19f1-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d19f1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
