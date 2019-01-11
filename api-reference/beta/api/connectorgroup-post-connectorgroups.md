---
title: Criar connectorGroup
description: Use essa API para criar um novo connectorGroup.
localization_priority: Normal
ms.openlocfilehash: 65fe6dd901de6238c450b4896b37d56fa8ea602f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824294"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="4bfdb-103">Criar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="4bfdb-103">Create connectorGroup</span></span>

> <span data-ttu-id="4bfdb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4bfdb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bfdb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4bfdb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4bfdb-106">Use essa API para criar um novo connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="4bfdb-106">Use this API to create a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bfdb-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="4bfdb-107">Permissions</span></span>
<span data-ttu-id="4bfdb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bfdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bfdb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bfdb-110">Permission type</span></span>      | <span data-ttu-id="4bfdb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4bfdb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bfdb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bfdb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4bfdb-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4bfdb-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4bfdb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bfdb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bfdb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bfdb-115">Not supported.</span></span>    |
|<span data-ttu-id="4bfdb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bfdb-116">Application</span></span> | <span data-ttu-id="4bfdb-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bfdb-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bfdb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bfdb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="4bfdb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bfdb-119">Request headers</span></span>
| <span data-ttu-id="4bfdb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4bfdb-120">Name</span></span>       | <span data-ttu-id="4bfdb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bfdb-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4bfdb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bfdb-122">Authorization</span></span>  | <span data-ttu-id="4bfdb-123">Portador.</span><span class="sxs-lookup"><span data-stu-id="4bfdb-123">Bearer.</span></span> <span data-ttu-id="4bfdb-124">Necessários</span><span class="sxs-lookup"><span data-stu-id="4bfdb-124">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bfdb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bfdb-125">Request body</span></span>
<span data-ttu-id="4bfdb-126">No corpo da solicitação, fornece uma representação JSON do objeto [connectorGroup](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="4bfdb-126">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4bfdb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bfdb-127">Response</span></span>

<span data-ttu-id="4bfdb-128">Se tiver êxito, este método retornará `201 Created` objeto response de código e [connectorGroup](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bfdb-128">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bfdb-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bfdb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bfdb-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bfdb-130">Request</span></span>
<span data-ttu-id="4bfdb-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bfdb-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connectorgroups"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```
<span data-ttu-id="4bfdb-132">No corpo da solicitação, fornece uma representação JSON do objeto [connectorGroup](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="4bfdb-132">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4bfdb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bfdb-133">Response</span></span>
<span data-ttu-id="4bfdb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bfdb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
