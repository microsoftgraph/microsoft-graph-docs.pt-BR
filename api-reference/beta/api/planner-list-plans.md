---
title: Listar planos
description: Recupere uma lista de objetos **plannerplan**.
ms.openlocfilehash: 830800463283b660ddeb4cd7d4fb4e4eb037c6ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041103"
---
# <a name="list-plans"></a><span data-ttu-id="0138e-103">Listar planos</span><span class="sxs-lookup"><span data-stu-id="0138e-103">List plans</span></span>

> <span data-ttu-id="0138e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0138e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0138e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0138e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0138e-106">Recupere uma lista de objetos **plannerplan**.</span><span class="sxs-lookup"><span data-stu-id="0138e-106">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="0138e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0138e-107">Permissions</span></span>
<span data-ttu-id="0138e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0138e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0138e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0138e-110">Permission type</span></span>      | <span data-ttu-id="0138e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0138e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0138e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0138e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0138e-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0138e-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0138e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0138e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0138e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0138e-115">Not supported.</span></span>    |
|<span data-ttu-id="0138e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0138e-116">Application</span></span> | <span data-ttu-id="0138e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0138e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0138e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0138e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0138e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0138e-119">Optional query parameters</span></span>
<span data-ttu-id="0138e-120">Este método requer que o [filtro](https://developer.microsoft.com/graph/docs/concepts/query_parameters) de proprietário seja especificado.</span><span class="sxs-lookup"><span data-stu-id="0138e-120">This method requires owner [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0138e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0138e-121">Request headers</span></span>
| <span data-ttu-id="0138e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0138e-122">Name</span></span>      |<span data-ttu-id="0138e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0138e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0138e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0138e-124">Authorization</span></span>  | <span data-ttu-id="0138e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0138e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0138e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0138e-127">Request body</span></span>
<span data-ttu-id="0138e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0138e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0138e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0138e-129">Response</span></span>

<span data-ttu-id="0138e-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0138e-130">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="0138e-p104">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="0138e-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="0138e-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0138e-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0138e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0138e-135">Request</span></span>
<span data-ttu-id="0138e-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0138e-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans
```
##### <a name="response"></a><span data-ttu-id="0138e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0138e-137">Response</span></span>
<span data-ttu-id="0138e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0138e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 421

{
  "value": [
    {
      "createdBy": {
        "application": {
          "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
        },
        "user": {
          "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
        }
      },
      "createdDateTime": "2015-03-30T18:36:49.2407981Z",
      "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
      "title": "title-value",
      "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->