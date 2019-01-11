---
title: Excluir administrativeUnit
description: Exclua um administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 7c90fda4bdcbb6a431dbcb4caa6a50a130c7f78b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860050"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="7e601-103">Excluir administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="7e601-103">Delete administrativeUnit</span></span>

> <span data-ttu-id="7e601-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7e601-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e601-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7e601-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7e601-106">Exclua um [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="7e601-106">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e601-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="7e601-107">Permissions</span></span>
<span data-ttu-id="7e601-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e601-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7e601-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e601-110">Permission type</span></span>      | <span data-ttu-id="7e601-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e601-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e601-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e601-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7e601-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7e601-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7e601-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e601-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e601-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e601-115">Not supported.</span></span>    |
|<span data-ttu-id="7e601-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e601-116">Application</span></span> | <span data-ttu-id="7e601-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e601-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e601-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e601-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7e601-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e601-119">Request headers</span></span>
| <span data-ttu-id="7e601-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7e601-120">Name</span></span>       | <span data-ttu-id="7e601-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e601-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7e601-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e601-122">Authorization</span></span>  | <span data-ttu-id="7e601-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e601-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e601-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e601-125">Request body</span></span>
<span data-ttu-id="7e601-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e601-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e601-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e601-127">Response</span></span>

<span data-ttu-id="7e601-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e601-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e601-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e601-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e601-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e601-131">Request</span></span>
<span data-ttu-id="7e601-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e601-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="7e601-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e601-133">Response</span></span>
<span data-ttu-id="7e601-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e601-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
