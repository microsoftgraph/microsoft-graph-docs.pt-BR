---
title: Lista recentPlans
description: Recupere uma lista de plannerPlans recentemente exibidos por um usuário. Você pode atualizar planos visualizados recentemente, atualizando o recurso plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.openlocfilehash: bfc2ffff15db55c289a95223ced6cb15af0535cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884487"
---
# <a name="list-recentplans"></a><span data-ttu-id="49db4-104">Lista recentPlans</span><span class="sxs-lookup"><span data-stu-id="49db4-104">List recentPlans</span></span>

> <span data-ttu-id="49db4-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="49db4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49db4-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="49db4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49db4-107">Recupere uma lista de [plannerPlans](../resources/plannerplan.md) recentemente exibidos por um usuário.</span><span class="sxs-lookup"><span data-stu-id="49db4-107">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="49db4-108">Você pode atualizar planos visualizados recentemente, [Atualizando o recurso plannerUser](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="49db4-108">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="49db4-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="49db4-109">Permissions</span></span>
<span data-ttu-id="49db4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49db4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49db4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49db4-112">Permission type</span></span>      | <span data-ttu-id="49db4-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49db4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49db4-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49db4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="49db4-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="49db4-115">Group.Read.All</span></span>    |
|<span data-ttu-id="49db4-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49db4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49db4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49db4-117">Not supported.</span></span>    |
|<span data-ttu-id="49db4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49db4-118">Application</span></span> | <span data-ttu-id="49db4-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49db4-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49db4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49db4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/<id>/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="49db4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49db4-121">Request headers</span></span>
| <span data-ttu-id="49db4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="49db4-122">Name</span></span>      |<span data-ttu-id="49db4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="49db4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49db4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="49db4-124">Authorization</span></span>  | <span data-ttu-id="49db4-p105">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49db4-p105">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49db4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49db4-127">Request body</span></span>
<span data-ttu-id="49db4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49db4-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="49db4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="49db4-129">Response</span></span>
<span data-ttu-id="49db4-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49db4-130">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49db4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49db4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49db4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49db4-132">Request</span></span>
<span data-ttu-id="49db4-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="49db4-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
##### <a name="response"></a><span data-ttu-id="49db4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="49db4-134">Response</span></span>
<span data-ttu-id="49db4-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="49db4-135">The following is an example of the response.</span></span> 

><span data-ttu-id="49db4-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49db4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtUGxhbiAgQEBAQEBAQEBAQEBAQEBDXCc=\"",
      "createdBy": {
        "user": {
          "id": "dd8a8379-1ac1-4eee-861d-ec15f6fa3611"
        },
        "application": {
          "id": "09abbdfd-ed23-44ee-a2d9-a627aa1c90f3"
        }
      },
      "createdDateTime": "2015-10-14T00:57:28.4698344Z",
      "owner": "eacd01dd-84cc-4c12-bd8a-9a33e5aeed11",
      "title": "Budget Planning (2016)",
      "id": "uZWtCtli30CGoWLIWSat1mQAC0ai"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List recentPlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
