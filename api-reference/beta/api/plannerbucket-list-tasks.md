---
title: Listar tarefas
description: Recupere uma lista de objetos **plannerTask** associados a um objeto plannerBucket.
ms.openlocfilehash: 679da04497cf17e64e7764abcbed5b4c9992bf9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037841"
---
# <a name="list-tasks"></a><span data-ttu-id="d7672-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="d7672-103">List tasks</span></span>

> <span data-ttu-id="d7672-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d7672-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7672-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d7672-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7672-106">Recupere uma lista de objetos **plannerTask** associados a um objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="d7672-106">Retrieve a list of **plannerTask** objects associated to a [plannerBucket](../resources/plannerbucket.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7672-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7672-107">Permissions</span></span>
<span data-ttu-id="d7672-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7672-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7672-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7672-110">Permission type</span></span>      | <span data-ttu-id="d7672-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7672-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7672-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7672-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7672-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7672-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d7672-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7672-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7672-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7672-115">Not supported.</span></span>    |
|<span data-ttu-id="d7672-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7672-116">Application</span></span> | <span data-ttu-id="d7672-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7672-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7672-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7672-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/<id>/tasks
```

## <a name="request-headers"></a><span data-ttu-id="d7672-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7672-119">Request headers</span></span>
| <span data-ttu-id="d7672-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d7672-120">Name</span></span>      |<span data-ttu-id="d7672-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7672-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d7672-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7672-122">Authorization</span></span>  | <span data-ttu-id="d7672-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7672-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7672-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7672-125">Request body</span></span>
<span data-ttu-id="d7672-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d7672-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7672-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7672-127">Response</span></span>

<span data-ttu-id="d7672-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7672-128">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="d7672-p104">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d7672-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d7672-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7672-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7672-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7672-133">Request</span></span>
<span data-ttu-id="d7672-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7672-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/planner/buckets/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/tasks
```
##### <a name="response"></a><span data-ttu-id="d7672-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7672-135">Response</span></span>
<span data-ttu-id="d7672-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7672-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 833

{
  "value": [
    {
      "createdBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
      "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
      "title": "title-value",
      "orderHint": "9223370609546166567W",
      "assigneePriority": "90057581\"",
      "createdDateTime": "2015-03-25T18:36:49.2407981Z",
      "assignments": {
        "fbab97d0-4932-4511-b675-204639209557": {
          "@odata.type": "#microsoft.graph.plannerassignment",
          "assignedBy": {
            "user": {
              "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
            }
          },
          "assignedDateTime": "2015-03-25T18:38:21.956Z",
          "orderHint": "RWk1"
         }
      },
      "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->