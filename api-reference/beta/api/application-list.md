---
title: Lista de aplicativos
description: Recupere a lista de aplicativos nesta organização.
author: lleonard-msft
localization_priority: Priority
ms.openlocfilehash: 5443010f613f1978c3b88a9cc57237ca7b844805
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854975"
---
# <a name="list-applications"></a><span data-ttu-id="9d80f-103">Lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="9d80f-103">List applications</span></span>

> <span data-ttu-id="9d80f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9d80f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d80f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9d80f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d80f-106">Recupere a lista de aplicativos nesta organização.</span><span class="sxs-lookup"><span data-stu-id="9d80f-106">Retrieve the list of applications in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d80f-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="9d80f-107">Permissions</span></span>
<span data-ttu-id="9d80f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d80f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9d80f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d80f-110">Permission type</span></span>      | <span data-ttu-id="9d80f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d80f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d80f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d80f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d80f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d80f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d80f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d80f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d80f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d80f-115">Not supported.</span></span>    |
|<span data-ttu-id="9d80f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d80f-116">Application</span></span> | <span data-ttu-id="9d80f-117">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d80f-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d80f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d80f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9d80f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9d80f-119">Optional query parameters</span></span>
<span data-ttu-id="9d80f-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9d80f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d80f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d80f-121">Request headers</span></span>
| <span data-ttu-id="9d80f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9d80f-122">Name</span></span>       | <span data-ttu-id="9d80f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d80f-123">Type</span></span> | <span data-ttu-id="9d80f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d80f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9d80f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d80f-125">Authorization</span></span>  | <span data-ttu-id="9d80f-126">string</span><span class="sxs-lookup"><span data-stu-id="9d80f-126">string</span></span>  | <span data-ttu-id="9d80f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d80f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9d80f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d80f-129">Request body</span></span>
<span data-ttu-id="9d80f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9d80f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d80f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d80f-131">Response</span></span>

<span data-ttu-id="9d80f-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de [aplicativo](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d80f-132">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d80f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d80f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d80f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d80f-134">Request</span></span>
<span data-ttu-id="9d80f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d80f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications
```
##### <a name="response"></a><span data-ttu-id="9d80f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d80f-136">Response</span></span>
<span data-ttu-id="9d80f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d80f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1229

{
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
