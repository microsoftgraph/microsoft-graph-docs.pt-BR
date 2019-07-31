---
title: Atribuir política
description: Atribui uma política a um aplicativo ou a uma entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: af128019d35838dd5873de713f011fd5b7f1c6ad
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978886"
---
# <a name="assign-policy"></a><span data-ttu-id="829f8-103">Atribuir política</span><span class="sxs-lookup"><span data-stu-id="829f8-103">Assign Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="829f8-104">Atribui uma [política](../resources/policy.md) a um aplicativo ou a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="829f8-104">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="829f8-105">Observação: no momento, a atribuição de política se aplica apenas à política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="829f8-105">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="829f8-106">Esse tipo de política é descrita na [política](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="829f8-106">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="829f8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="829f8-107">Permissions</span></span>
<span data-ttu-id="829f8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="829f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="829f8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="829f8-110">Permission type</span></span>      | <span data-ttu-id="829f8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="829f8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="829f8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="829f8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="829f8-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="829f8-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="829f8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="829f8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="829f8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="829f8-115">Not supported.</span></span>    |
|<span data-ttu-id="829f8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="829f8-116">Application</span></span> | <span data-ttu-id="829f8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="829f8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="829f8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="829f8-118">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="829f8-119">Observação: "ID" na solicitação é a propriedade "ID" da entidade de serviço ou aplicativo, não a propriedade "AppID".</span><span class="sxs-lookup"><span data-stu-id="829f8-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="829f8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="829f8-120">Request headers</span></span>
| <span data-ttu-id="829f8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="829f8-121">Name</span></span>       | <span data-ttu-id="829f8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="829f8-122">Type</span></span> | <span data-ttu-id="829f8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="829f8-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="829f8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="829f8-124">Authorization</span></span>  | <span data-ttu-id="829f8-125">string</span><span class="sxs-lookup"><span data-stu-id="829f8-125">string</span></span>  | <span data-ttu-id="829f8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="829f8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="829f8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="829f8-128">Content-Type</span></span> | <span data-ttu-id="829f8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="829f8-129">application/json</span></span>  | <span data-ttu-id="829f8-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="829f8-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="829f8-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="829f8-132">Request body</span></span>
<span data-ttu-id="829f8-133">No corpo da solicitação, forneça uma representação JSON do objeto Policy a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="829f8-133">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="829f8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="829f8-134">Response</span></span>

<span data-ttu-id="829f8-135">Quando é bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="829f8-135">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="829f8-136">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="829f8-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="829f8-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="829f8-137">Example</span></span>
<span data-ttu-id="829f8-138">O exemplo a seguir atribui uma política a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="829f8-138">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="829f8-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="829f8-139">Request</span></span>
<span data-ttu-id="829f8-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="829f8-140">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="829f8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="829f8-141">Response</span></span>
<span data-ttu-id="829f8-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="829f8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
