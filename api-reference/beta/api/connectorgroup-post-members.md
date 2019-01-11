---
title: Adicionar um conector para connectorGroup
description: Use essa API para adicionar um conector a um connectorGroup.
localization_priority: Normal
ms.openlocfilehash: 0624356699b5354ddc5f11740e8561a3d6e2d851
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869990"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="672d5-103">Adicionar um conector para connectorGroup</span><span class="sxs-lookup"><span data-stu-id="672d5-103">Add connector to connectorGroup</span></span>

> <span data-ttu-id="672d5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="672d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="672d5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="672d5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="672d5-106">Use essa API para adicionar um conector a um connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="672d5-106">Use this API to add a connector to a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="672d5-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="672d5-107">Permissions</span></span>
<span data-ttu-id="672d5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="672d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="672d5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="672d5-110">Permission type</span></span>      | <span data-ttu-id="672d5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="672d5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="672d5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="672d5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="672d5-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="672d5-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="672d5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="672d5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="672d5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="672d5-115">Not supported.</span></span>    |
|<span data-ttu-id="672d5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="672d5-116">Application</span></span> | <span data-ttu-id="672d5-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="672d5-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="672d5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="672d5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="672d5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="672d5-119">Request headers</span></span>
| <span data-ttu-id="672d5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="672d5-120">Name</span></span>       | <span data-ttu-id="672d5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="672d5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="672d5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="672d5-122">Authorization</span></span>  | <span data-ttu-id="672d5-123">Portador.</span><span class="sxs-lookup"><span data-stu-id="672d5-123">Bearer.</span></span> <span data-ttu-id="672d5-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="672d5-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="672d5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="672d5-125">Request body</span></span>
<span data-ttu-id="672d5-126">No corpo da solicitação, fornece uma representação JSON de um link para um objeto de [conector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="672d5-126">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="672d5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="672d5-127">Response</span></span>

<span data-ttu-id="672d5-128">Se tiver êxito, este método retornará `201 Created` objeto de [conector](../resources/connector.md) e o código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="672d5-128">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="672d5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="672d5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="672d5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="672d5-130">Request</span></span>
<span data-ttu-id="672d5-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="672d5-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connector_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups/{id}/members/$ref
Content-type: application/json
Content-length: 104

{
  "@odata.id": "https://graph.microsoft.com/{ver}/connector/{id}"
}
```
<span data-ttu-id="672d5-132">No corpo da solicitação, fornece uma representação JSON de um link para um objeto de [conector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="672d5-132">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="672d5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="672d5-133">Response</span></span>
<span data-ttu-id="672d5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="672d5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 124

{
  "id": "id-value",
  "machineName": "machineName-value",
  "externalIp": "externalIp-value",
  "status": "status-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
