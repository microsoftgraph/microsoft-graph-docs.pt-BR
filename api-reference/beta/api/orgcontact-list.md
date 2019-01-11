---
title: Lista orgContacts
description: Recupere a lista de contatos organizacionais para esta organização.
localization_priority: Normal
ms.openlocfilehash: 0b4dc4a099562b8817396bee8f3141fa32c28572
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831973"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="7e59e-103">Lista orgContacts</span><span class="sxs-lookup"><span data-stu-id="7e59e-103">List orgContacts</span></span>

> <span data-ttu-id="7e59e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7e59e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e59e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7e59e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7e59e-106">Recupere a lista de contatos organizacionais para esta organização.</span><span class="sxs-lookup"><span data-stu-id="7e59e-106">Retrieve the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e59e-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="7e59e-107">Permissions</span></span>
<span data-ttu-id="7e59e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e59e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e59e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e59e-110">Permission type</span></span>      | <span data-ttu-id="7e59e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e59e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e59e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e59e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7e59e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7e59e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7e59e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e59e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e59e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e59e-115">Not supported.</span></span>    |
|<span data-ttu-id="7e59e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e59e-116">Application</span></span> | <span data-ttu-id="7e59e-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e59e-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e59e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e59e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7e59e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7e59e-119">Optional query parameters</span></span>
<span data-ttu-id="7e59e-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7e59e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e59e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e59e-121">Request headers</span></span>
| <span data-ttu-id="7e59e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7e59e-122">Name</span></span>       | <span data-ttu-id="7e59e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e59e-123">Type</span></span> | <span data-ttu-id="7e59e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e59e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7e59e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e59e-125">Authorization</span></span>  | <span data-ttu-id="7e59e-126">string</span><span class="sxs-lookup"><span data-stu-id="7e59e-126">string</span></span>  | <span data-ttu-id="7e59e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e59e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e59e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e59e-129">Request body</span></span>
<span data-ttu-id="7e59e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e59e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e59e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e59e-131">Response</span></span>

<span data-ttu-id="7e59e-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e59e-132">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7e59e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e59e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e59e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e59e-134">Request</span></span>
<span data-ttu-id="7e59e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e59e-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts
```
##### <a name="response"></a><span data-ttu-id="7e59e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e59e-136">Response</span></span>
<span data-ttu-id="7e59e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e59e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "addresses":[
          {
            "city": "string",
            "countryOrRegion": "string",
            "officeLocation": "string",
            "postalCode": "string",
            "state": "string",
            "street": "string"
          }
      ],
      "companyName": "companyName-value",
      "department": "department-value",
      "displayName": "displayName-value",
      "phones":[
          {
            "type": "string",
            "number": "string"
          }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
