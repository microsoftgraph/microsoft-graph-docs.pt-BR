---
title: Atualizar oAuth2PermissionGrant
description: Atualize as propriedades do objeto oAuth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: 3c01d62dfb7c0c6906ff860656ee87b5f6d40aed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822348"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="9a4f7-103">Atualizar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="9a4f7-103">Update oAuth2PermissionGrant</span></span>

> <span data-ttu-id="9a4f7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9a4f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a4f7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9a4f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a4f7-106">Atualize as propriedades do objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="9a4f7-106">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a4f7-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="9a4f7-107">Permissions</span></span>

<span data-ttu-id="9a4f7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a4f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9a4f7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a4f7-110">Permission type</span></span>      | <span data-ttu-id="9a4f7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a4f7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a4f7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a4f7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9a4f7-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9a4f7-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a4f7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a4f7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a4f7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a4f7-115">Not supported.</span></span>    |
|<span data-ttu-id="9a4f7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a4f7-116">Application</span></span> | <span data-ttu-id="9a4f7-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a4f7-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a4f7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a4f7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9a4f7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a4f7-119">Request headers</span></span>
| <span data-ttu-id="9a4f7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9a4f7-120">Name</span></span>       | <span data-ttu-id="9a4f7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a4f7-121">Type</span></span> | <span data-ttu-id="9a4f7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a4f7-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9a4f7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a4f7-123">Authorization</span></span>  | <span data-ttu-id="9a4f7-124">string</span><span class="sxs-lookup"><span data-stu-id="9a4f7-124">string</span></span>  | <span data-ttu-id="9a4f7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a4f7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a4f7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a4f7-127">Request body</span></span>
<span data-ttu-id="9a4f7-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9a4f7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9a4f7-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a4f7-131">Property</span></span>     | <span data-ttu-id="9a4f7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a4f7-132">Type</span></span>   |<span data-ttu-id="9a4f7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a4f7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a4f7-134">scope</span><span class="sxs-lookup"><span data-stu-id="9a4f7-134">scope</span></span>|<span data-ttu-id="9a4f7-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a4f7-135">String</span></span>| <span data-ttu-id="9a4f7-136">Especifica o valor da declaração escopo que o aplicativo de recurso deve esperar que no token de acesso OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="9a4f7-136">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="9a4f7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a4f7-137">Response</span></span>

<span data-ttu-id="9a4f7-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a4f7-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a4f7-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a4f7-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a4f7-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a4f7-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_oAuth2Permissiongrant"
}-->
```http
PATCH https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
Content-type: application/json
Content-length: 30

{
  "scope": "scope-value"
}
```
##### <a name="response"></a><span data-ttu-id="9a4f7-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a4f7-142">Response</span></span>

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
  "description": "Update oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
