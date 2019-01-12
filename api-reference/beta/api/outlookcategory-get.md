---
title: Obter categoria do Outlook
description: Obtenha as propriedades e as relações do objeto outlookCategory especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c296aea62fec7090cb76607911f6be178f1ebdbb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949714"
---
# <a name="get-outlook-category"></a><span data-ttu-id="8b278-103">Obter categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="8b278-103">Get Outlook category</span></span>

> <span data-ttu-id="8b278-104">**Importante**: APIs sob a versão /beta no Microsoft Graph estiver em Visualizar e estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="8b278-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b278-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8b278-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b278-106">Obtenha as propriedades e as relações do objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="8b278-106">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b278-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b278-107">Permissions</span></span>
<span data-ttu-id="8b278-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b278-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b278-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b278-110">Permission type</span></span>      | <span data-ttu-id="8b278-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b278-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b278-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b278-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8b278-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="8b278-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="8b278-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b278-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b278-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="8b278-115">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="8b278-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b278-116">Application</span></span> | <span data-ttu-id="8b278-117">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="8b278-117">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b278-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b278-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8b278-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8b278-119">Optional query parameters</span></span>
<span data-ttu-id="8b278-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8b278-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b278-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b278-121">Request headers</span></span>
| <span data-ttu-id="8b278-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8b278-122">Name</span></span>      |<span data-ttu-id="8b278-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b278-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8b278-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b278-124">Authorization</span></span>  | <span data-ttu-id="8b278-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b278-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b278-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b278-127">Request body</span></span>
<span data-ttu-id="8b278-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8b278-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b278-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b278-129">Response</span></span>

<span data-ttu-id="8b278-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b278-130">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b278-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b278-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b278-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b278-132">Request</span></span>
<span data-ttu-id="8b278-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b278-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories('de912e4d-c790-4da9-949c-ccd933aaa0f7')
```
##### <a name="response"></a><span data-ttu-id="8b278-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b278-134">Response</span></span>
<span data-ttu-id="8b278-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b278-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 249

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
  "displayName":"Yellow category",
  "color":"preset3"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
