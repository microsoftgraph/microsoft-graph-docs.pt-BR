---
title: Listar aplicativos e entidades de serviço com política específica atribuída
description: Obter os objetos de entidade de serviço e aplicativo com a política especificada atribuída.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: 07d7a8cd1029de5205b1b2332d70bae868e6d614
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450869"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="74d27-103">Listar aplicativos e entidades de serviço com política específica atribuída</span><span class="sxs-lookup"><span data-stu-id="74d27-103">List applications and service principals with specific policy assigned</span></span>

<span data-ttu-id="74d27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74d27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74d27-105">Obter os objetos de [entidade de serviço](../resources/serviceprincipal.md) e [aplicativo](../resources/application.md) com a política especificada atribuída.</span><span class="sxs-lookup"><span data-stu-id="74d27-105">Get the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="74d27-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="74d27-106">Permissions</span></span>
<span data-ttu-id="74d27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74d27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74d27-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74d27-109">Permission type</span></span>      | <span data-ttu-id="74d27-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74d27-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74d27-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74d27-111">Delegated (work or school account)</span></span> | <span data-ttu-id="74d27-112">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="74d27-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="74d27-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74d27-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74d27-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74d27-114">Not supported.</span></span>    |
|<span data-ttu-id="74d27-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74d27-115">Application</span></span> | <span data-ttu-id="74d27-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="74d27-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74d27-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74d27-117">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="74d27-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74d27-118">Request headers</span></span>
| <span data-ttu-id="74d27-119">Nome</span><span class="sxs-lookup"><span data-stu-id="74d27-119">Name</span></span>       | <span data-ttu-id="74d27-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="74d27-120">Type</span></span> | <span data-ttu-id="74d27-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="74d27-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="74d27-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="74d27-122">Authorization</span></span>  | <span data-ttu-id="74d27-123">string</span><span class="sxs-lookup"><span data-stu-id="74d27-123">string</span></span>  | <span data-ttu-id="74d27-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74d27-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74d27-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74d27-126">Request body</span></span>
<span data-ttu-id="74d27-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74d27-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74d27-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="74d27-128">Response</span></span>

<span data-ttu-id="74d27-129">Se bem-sucedido, este método retorna `200 OK` o código de resposta e os objetos [Application](../resources/application.md) e [servicePrincipalName](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74d27-129">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="74d27-130">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="74d27-130">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="74d27-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74d27-131">Example</span></span>
<span data-ttu-id="74d27-132">O exemplo a seguir recupera os aplicativos e entidades de serviço com uma política específica atribuída.</span><span class="sxs-lookup"><span data-stu-id="74d27-132">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="74d27-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74d27-133">Request</span></span>
<span data-ttu-id="74d27-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74d27-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="74d27-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="74d27-135">Response</span></span>
<span data-ttu-id="74d27-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74d27-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
