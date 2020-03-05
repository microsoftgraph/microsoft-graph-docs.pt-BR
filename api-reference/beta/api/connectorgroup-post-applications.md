---
title: Criar aplicativo
description: Use esta API para criar um novo aplicativo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 018288444be3c2851e71117e1710a08947fa6104
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437354"
---
# <a name="create-application"></a><span data-ttu-id="0b963-103">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b963-103">Create application</span></span>

<span data-ttu-id="0b963-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0b963-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b963-105">Use esta API para criar um novo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0b963-105">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b963-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b963-106">Permissions</span></span>
<span data-ttu-id="0b963-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b963-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b963-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b963-109">Permission type</span></span>      | <span data-ttu-id="0b963-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b963-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b963-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b963-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b963-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0b963-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0b963-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b963-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b963-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b963-114">Not supported.</span></span>    |
|<span data-ttu-id="0b963-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b963-115">Application</span></span> | <span data-ttu-id="0b963-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b963-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b963-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b963-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="0b963-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b963-118">Request headers</span></span>
| <span data-ttu-id="0b963-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0b963-119">Name</span></span>       | <span data-ttu-id="0b963-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b963-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0b963-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b963-121">Authorization</span></span>  | <span data-ttu-id="0b963-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="0b963-122">Bearer.</span></span> <span data-ttu-id="0b963-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="0b963-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b963-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b963-124">Request body</span></span>
<span data-ttu-id="0b963-125">No corpo da solicitação, forneça uma representação JSON do objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="0b963-125">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0b963-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b963-126">Response</span></span>

<span data-ttu-id="0b963-127">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b963-127">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b963-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b963-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b963-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b963-129">Request</span></span>
<span data-ttu-id="0b963-130">Eis um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b963-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
Content-type: application/json
Content-length: 329

{
  "@odata.id": "https://graph.microsoft.com/{ver}/applications/{id}"
}
```
<span data-ttu-id="0b963-131">No corpo da solicitação, forneça uma representação JSON do objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="0b963-131">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0b963-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b963-132">Response</span></span>
<span data-ttu-id="0b963-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b963-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
