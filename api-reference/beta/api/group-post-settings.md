---
title: Criar uma configuração de diretório em grupos
description: Use essa API para criar uma nova configuração de diretório para o grupo.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 7db7072f683515ee1e5765d80184c6c284671eee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838581"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="6bfa6-103">Criar uma configuração de diretório em grupos</span><span class="sxs-lookup"><span data-stu-id="6bfa6-103">Create a directory setting on groups</span></span>

> <span data-ttu-id="6bfa6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6bfa6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bfa6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6bfa6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6bfa6-106">Use essa API para criar uma nova configuração de diretório para o grupo.</span><span class="sxs-lookup"><span data-stu-id="6bfa6-106">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="6bfa6-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="6bfa6-107">Permissions</span></span>
<span data-ttu-id="6bfa6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bfa6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bfa6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bfa6-110">Permission type</span></span>      | <span data-ttu-id="6bfa6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6bfa6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bfa6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bfa6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6bfa6-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6bfa6-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6bfa6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bfa6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bfa6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bfa6-115">Not supported.</span></span>    |
|<span data-ttu-id="6bfa6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bfa6-116">Application</span></span> | <span data-ttu-id="6bfa6-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bfa6-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bfa6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bfa6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="6bfa6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bfa6-119">Request headers</span></span>
| <span data-ttu-id="6bfa6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6bfa6-120">Name</span></span>       | <span data-ttu-id="6bfa6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bfa6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6bfa6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bfa6-122">Authorization</span></span>  | <span data-ttu-id="6bfa6-123">Portador <token>.</span><span class="sxs-lookup"><span data-stu-id="6bfa6-123">Bearer <token>.</span></span> <span data-ttu-id="6bfa6-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="6bfa6-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bfa6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bfa6-125">Request body</span></span>
<span data-ttu-id="6bfa6-126">No corpo da solicitação, fornece uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="6bfa6-126">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6bfa6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bfa6-127">Response</span></span>

<span data-ttu-id="6bfa6-128">Se tiver êxito, este método retornará `201 Created` objeto response de código e [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bfa6-128">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bfa6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bfa6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6bfa6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bfa6-130">Request</span></span>
<span data-ttu-id="6bfa6-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bfa6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/settings
Content-type: application/json
Content-length: 222

{
  "directorySetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```
<span data-ttu-id="6bfa6-132">No corpo da solicitação, fornece uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="6bfa6-132">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6bfa6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bfa6-133">Response</span></span>
<span data-ttu-id="6bfa6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bfa6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "directorySetting": {
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
