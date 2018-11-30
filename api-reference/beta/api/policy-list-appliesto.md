---
title: Lista de aplicativos e entidades de serviço com políticas específicas atribuídas
description: Recupere o aplicativo e objetos de entidades de serviço com a diretiva especificada atribuída.
ms.openlocfilehash: 3f281d7c60a506676a78637ad71f1ce26de35e34
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039577"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="6c43a-103">Lista de aplicativos e entidades de serviço com políticas específicas atribuídas</span><span class="sxs-lookup"><span data-stu-id="6c43a-103">List Applications and Service Principals with specific Policy assigned</span></span>

> <span data-ttu-id="6c43a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6c43a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c43a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6c43a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c43a-106">Recupere os objetos de [aplicativo](../resources/application.md) e [serviço principal](../resources/serviceprincipal.md) com a diretiva especificada atribuída.</span><span class="sxs-lookup"><span data-stu-id="6c43a-106">Retrieve the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c43a-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="6c43a-107">Permissions</span></span>
<span data-ttu-id="6c43a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c43a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c43a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c43a-110">Permission type</span></span>      | <span data-ttu-id="6c43a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c43a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c43a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c43a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6c43a-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6c43a-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6c43a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c43a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c43a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c43a-115">Not supported.</span></span>    |
|<span data-ttu-id="6c43a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c43a-116">Application</span></span> | <span data-ttu-id="6c43a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c43a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c43a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c43a-118">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="6c43a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c43a-119">Request headers</span></span>
| <span data-ttu-id="6c43a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6c43a-120">Name</span></span>       | <span data-ttu-id="6c43a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c43a-121">Type</span></span> | <span data-ttu-id="6c43a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c43a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6c43a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c43a-123">Authorization</span></span>  | <span data-ttu-id="6c43a-124">string</span><span class="sxs-lookup"><span data-stu-id="6c43a-124">string</span></span>  | <span data-ttu-id="6c43a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c43a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c43a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c43a-127">Request body</span></span>
<span data-ttu-id="6c43a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c43a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c43a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c43a-129">Response</span></span>

<span data-ttu-id="6c43a-130">Se tiver êxito, este método retornará `200 OK` objetos de código e o [aplicativo](../resources/application.md) e a [entidade de serviço](../resources/serviceprincipal.md) de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c43a-130">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="6c43a-131">Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="6c43a-131">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="6c43a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c43a-132">Example</span></span>
<span data-ttu-id="6c43a-133">O exemplo a seguir recupera os aplicativos e entidades de serviço com uma diretiva específica atribuída.</span><span class="sxs-lookup"><span data-stu-id="6c43a-133">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="6c43a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c43a-134">Request</span></span>
<span data-ttu-id="6c43a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c43a-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="6c43a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c43a-136">Response</span></span>
<span data-ttu-id="6c43a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c43a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value":[
        {
            "@odata.type"="#microsoft.graph.application",
            "appId":"appId-value",
            "displayName":"displayName-value",
            "errorUrl":"errorUrl-value",
            "groupMembershipClaims":"groupMembershipClaims-value",
            "homepage":"homepage-value",
            "id":"id-value",
            "keyCredentials":[key-credentials],
            "logoutUrl":"logoutUrl-value",
            "replyUrls":["replyUrls-value"]
        }
    ]
}
```
