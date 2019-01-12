---
title: Listar educationClasses
description: Recupera uma lista de classes de propriedade de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 40b86e4f392179ffb0c98ec0284d4d7c017dd930
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990450"
---
# <a name="list-educationclasses"></a><span data-ttu-id="f159f-103">Listar educationClasses</span><span class="sxs-lookup"><span data-stu-id="f159f-103">List educationClasses</span></span>

> <span data-ttu-id="f159f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f159f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f159f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f159f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f159f-106">Recupera uma lista de classes de propriedade de uma escola.</span><span class="sxs-lookup"><span data-stu-id="f159f-106">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="f159f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f159f-107">Permissions</span></span>
<span data-ttu-id="f159f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f159f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f159f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f159f-110">Permission type</span></span>      | <span data-ttu-id="f159f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f159f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f159f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f159f-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="f159f-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="f159f-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="f159f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f159f-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f159f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f159f-115">Not supported.</span></span>  |
|<span data-ttu-id="f159f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f159f-116">Application</span></span> | <span data-ttu-id="f159f-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f159f-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f159f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f159f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f159f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f159f-119">Optional query parameters</span></span>
<span data-ttu-id="f159f-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f159f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f159f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f159f-121">Request headers</span></span>
| <span data-ttu-id="f159f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f159f-122">Header</span></span>       | <span data-ttu-id="f159f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f159f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f159f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f159f-124">Authorization</span></span>  | <span data-ttu-id="f159f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f159f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f159f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f159f-127">Request body</span></span>
<span data-ttu-id="f159f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f159f-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f159f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f159f-129">Response</span></span>
<span data-ttu-id="f159f-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f159f-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f159f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f159f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f159f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f159f-132">Request</span></span>
<span data-ttu-id="f159f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f159f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/classes
```
##### <a name="response"></a><span data-ttu-id="f159f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f159f-134">Response</span></span>
<span data-ttu-id="f159f-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f159f-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f159f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f159f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    }  
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
