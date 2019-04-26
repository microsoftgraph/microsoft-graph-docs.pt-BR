---
title: Criar aplicativo
description: Use esta API para criar um novo aplicativo.
localization_priority: Normal
ms.openlocfilehash: ee0ecc6db99c0ea92131dbbf0e9c028234925f0a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327479"
---
# <a name="create-application"></a><span data-ttu-id="80df0-103">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="80df0-103">Create application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80df0-104">Use esta API para criar um novo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80df0-104">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="80df0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="80df0-105">Permissions</span></span>
<span data-ttu-id="80df0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80df0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80df0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80df0-108">Permission type</span></span>      | <span data-ttu-id="80df0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80df0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80df0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80df0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="80df0-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="80df0-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="80df0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80df0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80df0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80df0-113">Not supported.</span></span>    |
|<span data-ttu-id="80df0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80df0-114">Application</span></span> | <span data-ttu-id="80df0-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80df0-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80df0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80df0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="80df0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80df0-117">Request headers</span></span>
| <span data-ttu-id="80df0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="80df0-118">Name</span></span>       | <span data-ttu-id="80df0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="80df0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="80df0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="80df0-120">Authorization</span></span>  | <span data-ttu-id="80df0-121">Portador.</span><span class="sxs-lookup"><span data-stu-id="80df0-121">Bearer.</span></span> <span data-ttu-id="80df0-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="80df0-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="80df0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80df0-123">Request body</span></span>
<span data-ttu-id="80df0-124">No corpo da solicitação, forneça uma representação JSON do objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="80df0-124">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="80df0-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="80df0-125">Response</span></span>

<span data-ttu-id="80df0-126">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80df0-126">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80df0-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80df0-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80df0-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80df0-128">Request</span></span>
<span data-ttu-id="80df0-129">Eis um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80df0-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="80df0-130">No corpo da solicitação, forneça uma representação JSON do objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="80df0-130">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="80df0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="80df0-131">Response</span></span>
<span data-ttu-id="80df0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80df0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
