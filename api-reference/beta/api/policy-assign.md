---
title: Atribuir política
description: Atribui uma política a um aplicativo ou entidade de serviço.
localization_priority: Normal
ms.openlocfilehash: 30ba92c1d0308f9c4846702008a203821ae2b7b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865454"
---
# <a name="assign-policy"></a><span data-ttu-id="f653e-103">Atribuir política</span><span class="sxs-lookup"><span data-stu-id="f653e-103">Assign Policy</span></span>

> <span data-ttu-id="f653e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f653e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f653e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f653e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f653e-106">Atribui uma [política](../resources/policy.md) a um aplicativo ou entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="f653e-106">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="f653e-107">Observação: No momento, a atribuição da diretiva só se aplica a vida útil do Token política.</span><span class="sxs-lookup"><span data-stu-id="f653e-107">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="f653e-108">Esse tipo de política é descrito na [política](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="f653e-108">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f653e-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="f653e-109">Permissions</span></span>
<span data-ttu-id="f653e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f653e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f653e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f653e-112">Permission type</span></span>      | <span data-ttu-id="f653e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f653e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f653e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f653e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f653e-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f653e-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f653e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f653e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f653e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f653e-117">Not supported.</span></span>    |
|<span data-ttu-id="f653e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f653e-118">Application</span></span> | <span data-ttu-id="f653e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f653e-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f653e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f653e-120">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="f653e-121">Observação: O "id" na solicitação é a propriedade "id" do aplicativo ou serviço principal, não a propriedade "appid".</span><span class="sxs-lookup"><span data-stu-id="f653e-121">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f653e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f653e-122">Request headers</span></span>
| <span data-ttu-id="f653e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f653e-123">Name</span></span>       | <span data-ttu-id="f653e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f653e-124">Type</span></span> | <span data-ttu-id="f653e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f653e-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f653e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f653e-126">Authorization</span></span>  | <span data-ttu-id="f653e-127">string</span><span class="sxs-lookup"><span data-stu-id="f653e-127">string</span></span>  | <span data-ttu-id="f653e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f653e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f653e-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f653e-130">Content-Type</span></span> | <span data-ttu-id="f653e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f653e-131">application/json</span></span>  | <span data-ttu-id="f653e-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f653e-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f653e-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f653e-134">Request body</span></span>
<span data-ttu-id="f653e-135">No corpo da solicitação, fornecem uma representação de JSON do objeto de diretiva a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="f653e-135">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="f653e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f653e-136">Response</span></span>

<span data-ttu-id="f653e-137">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f653e-137">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="f653e-138">Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="f653e-138">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="f653e-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f653e-139">Example</span></span>
<span data-ttu-id="f653e-140">O exemplo a seguir atribui uma política a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f653e-140">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="f653e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f653e-141">Request</span></span>
<span data-ttu-id="f653e-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f653e-142">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="f653e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f653e-143">Response</span></span>
<span data-ttu-id="f653e-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f653e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
