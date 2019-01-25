---
title: Atribuir política
description: Atribui uma política a um aplicativo ou entidade de serviço.
localization_priority: Normal
ms.openlocfilehash: 15ba6a42f5c5d39caf57b25ebafc5dd4bc7990fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528211"
---
# <a name="assign-policy"></a><span data-ttu-id="d737e-103">Atribuir política</span><span class="sxs-lookup"><span data-stu-id="d737e-103">Assign Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d737e-104">Atribui uma [política](../resources/policy.md) a um aplicativo ou entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="d737e-104">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="d737e-105">Observação: No momento, a atribuição da diretiva só se aplica a vida útil do Token política.</span><span class="sxs-lookup"><span data-stu-id="d737e-105">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="d737e-106">Esse tipo de política é descrito na [política](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="d737e-106">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d737e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d737e-107">Permissions</span></span>
<span data-ttu-id="d737e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d737e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d737e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d737e-110">Permission type</span></span>      | <span data-ttu-id="d737e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d737e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d737e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d737e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d737e-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d737e-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d737e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d737e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d737e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d737e-115">Not supported.</span></span>    |
|<span data-ttu-id="d737e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d737e-116">Application</span></span> | <span data-ttu-id="d737e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d737e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d737e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d737e-118">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="d737e-119">Observação: O "id" na solicitação é a propriedade "id" do aplicativo ou serviço principal, não a propriedade "appid".</span><span class="sxs-lookup"><span data-stu-id="d737e-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d737e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d737e-120">Request headers</span></span>
| <span data-ttu-id="d737e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d737e-121">Name</span></span>       | <span data-ttu-id="d737e-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d737e-122">Type</span></span> | <span data-ttu-id="d737e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d737e-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d737e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d737e-124">Authorization</span></span>  | <span data-ttu-id="d737e-125">string</span><span class="sxs-lookup"><span data-stu-id="d737e-125">string</span></span>  | <span data-ttu-id="d737e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d737e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d737e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d737e-128">Content-Type</span></span> | <span data-ttu-id="d737e-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d737e-129">application/json</span></span>  | <span data-ttu-id="d737e-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d737e-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d737e-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d737e-132">Request body</span></span>
<span data-ttu-id="d737e-133">No corpo da solicitação, fornecem uma representação de JSON do objeto de diretiva a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="d737e-133">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="d737e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d737e-134">Response</span></span>

<span data-ttu-id="d737e-135">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d737e-135">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="d737e-136">Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="d737e-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="d737e-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d737e-137">Example</span></span>
<span data-ttu-id="d737e-138">O exemplo a seguir atribui uma política a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d737e-138">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="d737e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d737e-139">Request</span></span>
<span data-ttu-id="d737e-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d737e-140">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="d737e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d737e-141">Response</span></span>
<span data-ttu-id="d737e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d737e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-assign.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
