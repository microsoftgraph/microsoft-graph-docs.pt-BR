---
title: Adicionar um aplicativo a um conector
description: Use esta API para atribuir um aplicativo a um grupo de conectores
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0278810a70f8054688a8e1258cb9d50b6ed7a28d
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681260"
---
# <a name="add-an-application-to-a-connectorgroup"></a><span data-ttu-id="2db24-103">Adicionar um aplicativo a um conector</span><span class="sxs-lookup"><span data-stu-id="2db24-103">Add an application to a connectorGroup</span></span>

<span data-ttu-id="2db24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2db24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2db24-105">Adicionar um [aplicativo](../resources/application.md) a um [conector](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="2db24-105">Add an [application](../resources/application.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2db24-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2db24-106">Permissions</span></span>
<span data-ttu-id="2db24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2db24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2db24-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2db24-109">Permission type</span></span>      | <span data-ttu-id="2db24-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2db24-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2db24-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2db24-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2db24-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2db24-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2db24-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2db24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2db24-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2db24-114">Not supported.</span></span>    |
|<span data-ttu-id="2db24-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2db24-115">Application</span></span> | <span data-ttu-id="2db24-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2db24-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="2db24-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2db24-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="2db24-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2db24-118">Request headers</span></span>
| <span data-ttu-id="2db24-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2db24-119">Name</span></span>       | <span data-ttu-id="2db24-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2db24-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2db24-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2db24-121">Authorization</span></span>  | <span data-ttu-id="2db24-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="2db24-122">Bearer.</span></span> <span data-ttu-id="2db24-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="2db24-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="2db24-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2db24-124">Request body</span></span>
<span data-ttu-id="2db24-125">No corpo da solicitação, forneça uma representação JSON do objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="2db24-125">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2db24-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2db24-126">Response</span></span>

<span data-ttu-id="2db24-127">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2db24-127">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2db24-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2db24-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2db24-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2db24-129">Request</span></span>
<span data-ttu-id="2db24-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2db24-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2db24-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2db24-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
Content-type: application/json
Content-length: 329

{
  "@odata.id": "https://graph.microsoft.com/beta/applications/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="2db24-132">C#</span><span class="sxs-lookup"><span data-stu-id="2db24-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2db24-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2db24-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2db24-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2db24-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2db24-135">No corpo da solicitação, forneça uma representação JSON do objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="2db24-135">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2db24-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2db24-136">Response</span></span>
<span data-ttu-id="2db24-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2db24-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 355

{
  "appId": "appId-value",
  "onPremisesPublishing": {
    "externalUrl": "externalUrl-value",
    "internalUrl": "internalUrl-value",
    "externalAuthenticationType": "externalAuthenticationType-value",
    "customDomainCertificate": "customDomainCertificate-value",
    "isTranslateHostHeaderEnabled": true,
    "isOnPremPublishingEnabled": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
