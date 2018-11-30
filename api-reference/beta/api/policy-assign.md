---
title: Atribuir política
description: Atribui uma política a um aplicativo ou entidade de serviço.
ms.openlocfilehash: 25dee4ac43716949125795114318d2571d5b8647
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039578"
---
# <a name="assign-policy"></a><span data-ttu-id="ca21c-103">Atribuir política</span><span class="sxs-lookup"><span data-stu-id="ca21c-103">Assign Policy</span></span>

> <span data-ttu-id="ca21c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ca21c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca21c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ca21c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca21c-106">Atribui uma [política](../resources/policy.md) a um aplicativo ou entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="ca21c-106">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="ca21c-107">Observação: No momento, a atribuição da diretiva só se aplica a vida útil do Token política.</span><span class="sxs-lookup"><span data-stu-id="ca21c-107">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="ca21c-108">Esse tipo de política é descrito na [política](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="ca21c-108">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca21c-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="ca21c-109">Permissions</span></span>
<span data-ttu-id="ca21c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca21c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca21c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca21c-112">Permission type</span></span>      | <span data-ttu-id="ca21c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca21c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca21c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca21c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ca21c-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca21c-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca21c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca21c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca21c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca21c-117">Not supported.</span></span>    |
|<span data-ttu-id="ca21c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca21c-118">Application</span></span> | <span data-ttu-id="ca21c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca21c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca21c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca21c-120">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="ca21c-121">Observação: O "id" na solicitação é a propriedade "id" do aplicativo ou serviço principal, não a propriedade "appid".</span><span class="sxs-lookup"><span data-stu-id="ca21c-121">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca21c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca21c-122">Request headers</span></span>
| <span data-ttu-id="ca21c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ca21c-123">Name</span></span>       | <span data-ttu-id="ca21c-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca21c-124">Type</span></span> | <span data-ttu-id="ca21c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca21c-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ca21c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca21c-126">Authorization</span></span>  | <span data-ttu-id="ca21c-127">string</span><span class="sxs-lookup"><span data-stu-id="ca21c-127">string</span></span>  | <span data-ttu-id="ca21c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca21c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca21c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca21c-130">Content-Type</span></span> | <span data-ttu-id="ca21c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="ca21c-131">application/json</span></span>  | <span data-ttu-id="ca21c-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca21c-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca21c-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca21c-134">Request body</span></span>
<span data-ttu-id="ca21c-135">No corpo da solicitação, fornecem uma representação de JSON do objeto de diretiva a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="ca21c-135">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="ca21c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca21c-136">Response</span></span>

<span data-ttu-id="ca21c-137">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ca21c-137">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="ca21c-138">Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="ca21c-138">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="ca21c-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca21c-139">Example</span></span>
<span data-ttu-id="ca21c-140">O exemplo a seguir atribui uma política a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca21c-140">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="ca21c-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca21c-141">Request</span></span>
<span data-ttu-id="ca21c-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca21c-142">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="ca21c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca21c-143">Response</span></span>
<span data-ttu-id="ca21c-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca21c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
