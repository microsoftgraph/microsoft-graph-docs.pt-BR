---
title: Criar aplicativo
description: Use essa API para criar um novo aplicativo.
ms.openlocfilehash: 08300057f78671ce74dd98bd98f7d3182bde083d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036256"
---
# <a name="create-application"></a><span data-ttu-id="60860-103">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="60860-103">Create application</span></span>

> <span data-ttu-id="60860-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="60860-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60860-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="60860-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60860-106">Use essa API para criar um novo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="60860-106">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="60860-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="60860-107">Permissions</span></span>
<span data-ttu-id="60860-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60860-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60860-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60860-110">Permission type</span></span>      | <span data-ttu-id="60860-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60860-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60860-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60860-112">Delegated (work or school account)</span></span> | <span data-ttu-id="60860-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="60860-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="60860-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60860-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60860-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60860-115">Not supported.</span></span>    |
|<span data-ttu-id="60860-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60860-116">Application</span></span> | <span data-ttu-id="60860-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60860-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60860-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60860-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="60860-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60860-119">Request headers</span></span>
| <span data-ttu-id="60860-120">Nome</span><span class="sxs-lookup"><span data-stu-id="60860-120">Name</span></span>       | <span data-ttu-id="60860-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="60860-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="60860-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="60860-122">Authorization</span></span>  | <span data-ttu-id="60860-123">Portador.</span><span class="sxs-lookup"><span data-stu-id="60860-123">Bearer.</span></span> <span data-ttu-id="60860-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="60860-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="60860-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60860-125">Request body</span></span>
<span data-ttu-id="60860-126">No corpo da solicitação, fornece uma representação JSON do objeto [application](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="60860-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="60860-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="60860-127">Response</span></span>

<span data-ttu-id="60860-128">Se tiver êxito, este método retornará `201 Created` objeto de códigos e [aplicativos](../resources/application.md) de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60860-128">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60860-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60860-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60860-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60860-130">Request</span></span>
<span data-ttu-id="60860-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60860-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="60860-132">No corpo da solicitação, fornece uma representação JSON do objeto [application](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="60860-132">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="60860-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="60860-133">Response</span></span>
<span data-ttu-id="60860-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60860-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
