---
title: Lista de aplicativos e entidades de serviço com políticas específicas atribuídas
description: Recupere o aplicativo e objetos de entidades de serviço com a diretiva especificada atribuída.
localization_priority: Normal
ms.openlocfilehash: d7449428216a2e68d9ab8bb8399ca0e8dc4b72fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510474"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="ef4e0-103">Lista de aplicativos e entidades de serviço com políticas específicas atribuídas</span><span class="sxs-lookup"><span data-stu-id="ef4e0-103">List Applications and Service Principals with specific Policy assigned</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef4e0-104">Recupere os objetos de [aplicativo](../resources/application.md) e [serviço principal](../resources/serviceprincipal.md) com a diretiva especificada atribuída.</span><span class="sxs-lookup"><span data-stu-id="ef4e0-104">Retrieve the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef4e0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef4e0-105">Permissions</span></span>
<span data-ttu-id="ef4e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef4e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef4e0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef4e0-108">Permission type</span></span>      | <span data-ttu-id="ef4e0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef4e0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef4e0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef4e0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ef4e0-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ef4e0-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ef4e0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef4e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef4e0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef4e0-113">Not supported.</span></span>    |
|<span data-ttu-id="ef4e0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef4e0-114">Application</span></span> | <span data-ttu-id="ef4e0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef4e0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef4e0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef4e0-116">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="ef4e0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4e0-117">Request headers</span></span>
| <span data-ttu-id="ef4e0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ef4e0-118">Name</span></span>       | <span data-ttu-id="ef4e0-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef4e0-119">Type</span></span> | <span data-ttu-id="ef4e0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef4e0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ef4e0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef4e0-121">Authorization</span></span>  | <span data-ttu-id="ef4e0-122">string</span><span class="sxs-lookup"><span data-stu-id="ef4e0-122">string</span></span>  | <span data-ttu-id="ef4e0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef4e0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef4e0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4e0-125">Request body</span></span>
<span data-ttu-id="ef4e0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ef4e0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef4e0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef4e0-127">Response</span></span>

<span data-ttu-id="ef4e0-128">Se tiver êxito, este método retornará `200 OK` objetos de código e o [aplicativo](../resources/application.md) e a [entidade de serviço](../resources/serviceprincipal.md) de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef4e0-128">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="ef4e0-129">Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="ef4e0-129">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="ef4e0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef4e0-130">Example</span></span>
<span data-ttu-id="ef4e0-131">O exemplo a seguir recupera os aplicativos e entidades de serviço com uma diretiva específica atribuída.</span><span class="sxs-lookup"><span data-stu-id="ef4e0-131">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="ef4e0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4e0-132">Request</span></span>
<span data-ttu-id="ef4e0-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef4e0-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="ef4e0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef4e0-134">Response</span></span>
<span data-ttu-id="ef4e0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef4e0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-list-appliesto.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
