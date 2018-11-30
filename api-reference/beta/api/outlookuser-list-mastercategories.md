---
title: Listar categorias do Outlook
description: Obtém todas as categorias que foram definidas para o usuário.
ms.openlocfilehash: 7eff66ea876c88e6a75953f4bd219e817a9a2e2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038483"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="58cce-103">Listar categorias do Outlook</span><span class="sxs-lookup"><span data-stu-id="58cce-103">List Outlook categories</span></span>

> <span data-ttu-id="58cce-104">**Importante**: APIs sob a versão /beta no Microsoft Graph estiver em Visualizar e estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="58cce-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58cce-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="58cce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="58cce-106">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="58cce-106">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="58cce-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="58cce-107">Permissions</span></span>
<span data-ttu-id="58cce-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58cce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58cce-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58cce-110">Permission type</span></span>      | <span data-ttu-id="58cce-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58cce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58cce-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58cce-112">Delegated (work or school account)</span></span> | <span data-ttu-id="58cce-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="58cce-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="58cce-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58cce-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58cce-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="58cce-115">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="58cce-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58cce-116">Application</span></span> | <span data-ttu-id="58cce-117">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="58cce-117">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="58cce-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58cce-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="58cce-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58cce-119">Optional query parameters</span></span>
<span data-ttu-id="58cce-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="58cce-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58cce-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58cce-121">Request headers</span></span>
| <span data-ttu-id="58cce-122">Nome</span><span class="sxs-lookup"><span data-stu-id="58cce-122">Name</span></span>      |<span data-ttu-id="58cce-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="58cce-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="58cce-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="58cce-124">Authorization</span></span>  | <span data-ttu-id="58cce-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58cce-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58cce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58cce-127">Request body</span></span>
<span data-ttu-id="58cce-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58cce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58cce-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="58cce-129">Response</span></span>

<span data-ttu-id="58cce-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58cce-130">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="58cce-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58cce-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58cce-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58cce-132">Request</span></span>
<span data-ttu-id="58cce-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58cce-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories
```
##### <a name="response"></a><span data-ttu-id="58cce-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="58cce-134">Response</span></span>
<span data-ttu-id="58cce-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58cce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories",
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