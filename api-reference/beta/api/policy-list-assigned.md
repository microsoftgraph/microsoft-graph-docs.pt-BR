---
title: Listar políticas atribuídas à entidade de serviço ou aplicativo
description: Recupere os objetos de política atribuídos a uma entidade de serviço ou aplicativo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 06eb805b6983c72c14c86780f081554611906181
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992049"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="dfc35-103">Listar políticas atribuídas à entidade de serviço ou aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfc35-103">List Policies assigned to Application or Service Principal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfc35-104">Recupere os objetos de [política](../resources/policy.md) atribuídos a uma entidade de serviço ou aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dfc35-104">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfc35-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfc35-105">Permissions</span></span>
<span data-ttu-id="dfc35-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfc35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfc35-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfc35-108">Permission type</span></span>      | <span data-ttu-id="dfc35-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfc35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfc35-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfc35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dfc35-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dfc35-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dfc35-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfc35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfc35-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfc35-113">Not supported.</span></span>    |
|<span data-ttu-id="dfc35-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfc35-114">Application</span></span> | <span data-ttu-id="dfc35-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfc35-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfc35-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfc35-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="dfc35-117">Observação: "ID" na solicitação é a propriedade "ID" da entidade de serviço ou aplicativo, não a propriedade "AppID".</span><span class="sxs-lookup"><span data-stu-id="dfc35-117">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfc35-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc35-118">Request headers</span></span>
| <span data-ttu-id="dfc35-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dfc35-119">Name</span></span>       | <span data-ttu-id="dfc35-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfc35-120">Type</span></span> | <span data-ttu-id="dfc35-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfc35-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dfc35-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfc35-122">Authorization</span></span>  | <span data-ttu-id="dfc35-123">string</span><span class="sxs-lookup"><span data-stu-id="dfc35-123">string</span></span>  | <span data-ttu-id="dfc35-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfc35-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfc35-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc35-126">Request body</span></span>
<span data-ttu-id="dfc35-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfc35-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfc35-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfc35-128">Response</span></span>

<span data-ttu-id="dfc35-129">Se bem-sucedido, este método retorna `200 OK` o código de resposta e os objetos [Policy](../resources/policy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfc35-129">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="dfc35-130">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="dfc35-130">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="dfc35-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfc35-131">Example</span></span>
<span data-ttu-id="dfc35-132">O exemplo a seguir recupera as políticas atribuídas a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dfc35-132">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="dfc35-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc35-133">Request</span></span>
<span data-ttu-id="dfc35-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfc35-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="dfc35-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfc35-135">Response</span></span>
<span data-ttu-id="dfc35-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfc35-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: application/json

{
    "value":[
        {
            "@odata.type":"#microsoft.graph.policy",
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault":boolean-value,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
