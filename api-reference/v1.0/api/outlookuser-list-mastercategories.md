---
title: Listar categorias do Outlook
description: Obtém todas as categorias que foram definidas para o usuário.
ms.openlocfilehash: a27d8083a3a19e14d4c077e97c32525925538997
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004156"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="ff418-103">Listar categorias do Outlook</span><span class="sxs-lookup"><span data-stu-id="ff418-103">List Outlook categories</span></span>


<span data-ttu-id="ff418-104">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="ff418-104">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff418-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff418-105">Permissions</span></span>
<span data-ttu-id="ff418-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff418-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff418-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff418-108">Permission type</span></span>      | <span data-ttu-id="ff418-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff418-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff418-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff418-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff418-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ff418-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="ff418-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff418-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff418-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ff418-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="ff418-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff418-114">Application</span></span> | <span data-ttu-id="ff418-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ff418-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff418-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff418-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ff418-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ff418-117">Optional query parameters</span></span>
<span data-ttu-id="ff418-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ff418-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff418-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff418-119">Request headers</span></span>
| <span data-ttu-id="ff418-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ff418-120">Name</span></span>      |<span data-ttu-id="ff418-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff418-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ff418-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff418-122">Authorization</span></span>  | <span data-ttu-id="ff418-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff418-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff418-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff418-125">Request body</span></span>
<span data-ttu-id="ff418-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff418-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff418-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff418-127">Response</span></span>

<span data-ttu-id="ff418-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff418-128">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff418-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff418-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff418-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff418-130">Request</span></span>
<span data-ttu-id="ff418-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff418-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories
```
##### <a name="response"></a><span data-ttu-id="ff418-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff418-132">Response</span></span>
<span data-ttu-id="ff418-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff418-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 727

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories",
  "value":[
    {
      "id":"5a9a6aa8-b65f-4357-b1f9-60c6bf6330d8",
      "displayName":"Red category",
      "color":"preset0"
    },
    {
      "id":"4b1c2495-54c9-4a5e-90a2-0ab0b31987d8",
      "displayName":"Orange category",
      "color":"preset1"
    },
    {
      "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
      "displayName":"Yellow category",
      "color":"preset3"
    },
    {
      "id":"79c8d8f8-9db1-49ec-99ce-ae25793e7232",
      "displayName":"Green category",
      "color":"preset4"
    },
    {
      "id":"626e696c-6a10-48b8-89b9-12de3160cfb9",
      "displayName":"Blue category",
      "color":"preset7"
    },
    {
      "id":"453d06d0-447d-41f7-91cd-aa0f6b190b5b",
      "displayName":"Purple category",
      "color":"preset8"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->