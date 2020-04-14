---
title: Atribuir política
description: Atribui uma política a um aplicativo ou a uma entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: 694b070b0186e8e76a0bb7180e538c0ac42188d8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450890"
---
# <a name="assign-policy"></a><span data-ttu-id="e6365-103">Atribuir política</span><span class="sxs-lookup"><span data-stu-id="e6365-103">Assign Policy</span></span>

<span data-ttu-id="e6365-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6365-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6365-105">Atribui uma [política](../resources/policy.md) a um aplicativo ou a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="e6365-105">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="e6365-106">Observação: no momento, a atribuição de política se aplica apenas à política de tempo de vida do token.</span><span class="sxs-lookup"><span data-stu-id="e6365-106">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="e6365-107">Esse tipo de política é descrita na [política](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="e6365-107">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6365-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6365-108">Permissions</span></span>
<span data-ttu-id="e6365-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6365-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6365-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6365-111">Permission type</span></span>      | <span data-ttu-id="e6365-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6365-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6365-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6365-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e6365-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6365-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6365-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6365-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6365-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6365-116">Not supported.</span></span>    |
|<span data-ttu-id="e6365-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6365-117">Application</span></span> | <span data-ttu-id="e6365-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6365-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6365-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6365-119">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="e6365-120">Observação: "ID" na solicitação é a propriedade "ID" da entidade de serviço ou aplicativo, não a propriedade "AppID".</span><span class="sxs-lookup"><span data-stu-id="e6365-120">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6365-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6365-121">Request headers</span></span>
| <span data-ttu-id="e6365-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e6365-122">Name</span></span>       | <span data-ttu-id="e6365-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6365-123">Type</span></span> | <span data-ttu-id="e6365-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6365-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6365-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6365-125">Authorization</span></span>  | <span data-ttu-id="e6365-126">string</span><span class="sxs-lookup"><span data-stu-id="e6365-126">string</span></span>  | <span data-ttu-id="e6365-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6365-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6365-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6365-129">Content-Type</span></span> | <span data-ttu-id="e6365-130">application/json</span><span class="sxs-lookup"><span data-stu-id="e6365-130">application/json</span></span>  | <span data-ttu-id="e6365-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6365-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6365-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6365-133">Request body</span></span>
<span data-ttu-id="e6365-134">No corpo da solicitação, forneça uma representação JSON do objeto Policy a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="e6365-134">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="e6365-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6365-135">Response</span></span>

<span data-ttu-id="e6365-136">Quando é bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e6365-136">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="e6365-137">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="e6365-137">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="e6365-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6365-138">Example</span></span>
<span data-ttu-id="e6365-139">O exemplo a seguir atribui uma política a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6365-139">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="e6365-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6365-140">Request</span></span>
<span data-ttu-id="e6365-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6365-141">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="e6365-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6365-142">Response</span></span>
<span data-ttu-id="e6365-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6365-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
