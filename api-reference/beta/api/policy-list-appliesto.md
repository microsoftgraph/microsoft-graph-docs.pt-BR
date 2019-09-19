---
title: Listar aplicativos e entidades de serviço com política específica atribuída
description: Obter os objetos de entidade de serviço e aplicativo com a política especificada atribuída.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 2158c1183bcbf036c7b4b429675d70b0a0b175de
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036134"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="427a5-103">Listar aplicativos e entidades de serviço com política específica atribuída</span><span class="sxs-lookup"><span data-stu-id="427a5-103">List applications and service principals with specific policy assigned</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="427a5-104">Obter os objetos de [entidade de serviço](../resources/serviceprincipal.md) e [aplicativo](../resources/application.md) com a política especificada atribuída.</span><span class="sxs-lookup"><span data-stu-id="427a5-104">Get the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="427a5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="427a5-105">Permissions</span></span>
<span data-ttu-id="427a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="427a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="427a5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="427a5-108">Permission type</span></span>      | <span data-ttu-id="427a5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="427a5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="427a5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="427a5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="427a5-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="427a5-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="427a5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="427a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="427a5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="427a5-113">Not supported.</span></span>    |
|<span data-ttu-id="427a5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="427a5-114">Application</span></span> | <span data-ttu-id="427a5-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="427a5-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="427a5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="427a5-116">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="427a5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="427a5-117">Request headers</span></span>
| <span data-ttu-id="427a5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="427a5-118">Name</span></span>       | <span data-ttu-id="427a5-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="427a5-119">Type</span></span> | <span data-ttu-id="427a5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="427a5-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="427a5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="427a5-121">Authorization</span></span>  | <span data-ttu-id="427a5-122">string</span><span class="sxs-lookup"><span data-stu-id="427a5-122">string</span></span>  | <span data-ttu-id="427a5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="427a5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="427a5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="427a5-125">Request body</span></span>
<span data-ttu-id="427a5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="427a5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="427a5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="427a5-127">Response</span></span>

<span data-ttu-id="427a5-128">Se bem-sucedido, este método retorna `200 OK` o código de resposta e os objetos [Application](../resources/application.md) e [servicePrincipalName](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="427a5-128">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="427a5-129">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="427a5-129">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="427a5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="427a5-130">Example</span></span>
<span data-ttu-id="427a5-131">O exemplo a seguir recupera os aplicativos e entidades de serviço com uma política específica atribuída.</span><span class="sxs-lookup"><span data-stu-id="427a5-131">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="427a5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="427a5-132">Request</span></span>
<span data-ttu-id="427a5-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="427a5-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="427a5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="427a5-134">Response</span></span>
<span data-ttu-id="427a5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="427a5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
