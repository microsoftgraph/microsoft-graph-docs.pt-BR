---
title: Excluir privilegedRoleAssignment
description: Exclua privilegedRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 10d8b10522f26c386e918fb1806c1807d28314e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888939"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="a51ab-103">Excluir privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a51ab-103">Delete privilegedRoleAssignment</span></span>

> <span data-ttu-id="a51ab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a51ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a51ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a51ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a51ab-106">Exclua [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a51ab-106">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a51ab-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="a51ab-107">Permissions</span></span>
<span data-ttu-id="a51ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a51ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a51ab-110">O solicitante precisa ter a função de _Administrador com privilégios de função_ .</span><span class="sxs-lookup"><span data-stu-id="a51ab-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="a51ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a51ab-111">Permission type</span></span>      | <span data-ttu-id="a51ab-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a51ab-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a51ab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a51ab-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a51ab-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a51ab-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a51ab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a51ab-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a51ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a51ab-116">Not supported.</span></span>    |
|<span data-ttu-id="a51ab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a51ab-117">Application</span></span> | <span data-ttu-id="a51ab-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a51ab-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a51ab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a51ab-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="a51ab-120">Observe que ``<id>`` está no formato de 'userId_roleId', onde userId é a cadeia de caracteres do GUID para id de usuário do Windows Azure AD e roleId é a cadeia de caracteres do GUID para id de função de administrador do Azure.</span><span class="sxs-lookup"><span data-stu-id="a51ab-120">Note that ``<id>`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a51ab-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a51ab-121">Request headers</span></span>
| <span data-ttu-id="a51ab-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a51ab-122">Name</span></span>       | <span data-ttu-id="a51ab-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a51ab-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a51ab-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a51ab-124">Authorization</span></span>  | <span data-ttu-id="a51ab-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a51ab-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a51ab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a51ab-127">Request body</span></span>
<span data-ttu-id="a51ab-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a51ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a51ab-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a51ab-129">Response</span></span>

<span data-ttu-id="a51ab-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a51ab-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="a51ab-132">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="a51ab-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a51ab-133">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="a51ab-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="a51ab-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a51ab-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a51ab-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a51ab-135">Request</span></span>
<span data-ttu-id="a51ab-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a51ab-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="a51ab-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a51ab-137">Response</span></span>
<span data-ttu-id="a51ab-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a51ab-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
