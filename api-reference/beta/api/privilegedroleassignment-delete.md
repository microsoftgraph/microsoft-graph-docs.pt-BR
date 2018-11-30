---
title: Excluir privilegedRoleAssignment
description: Exclua privilegedRoleAssignment.
ms.openlocfilehash: 345ebbfbf32a8d5e6f9399e5746ca9ece9b91d3b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034424"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="8c9f4-103">Excluir privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8c9f4-103">Delete privilegedRoleAssignment</span></span>

> <span data-ttu-id="8c9f4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8c9f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c9f4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8c9f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8c9f4-106">Exclua [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8c9f4-106">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="8c9f4-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8c9f4-107">Permissions</span></span>
<span data-ttu-id="8c9f4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c9f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8c9f4-110">O solicitante precisa ter a função de _Administrador com privilégios de função_ .</span><span class="sxs-lookup"><span data-stu-id="8c9f4-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="8c9f4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c9f4-111">Permission type</span></span>      | <span data-ttu-id="8c9f4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c9f4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c9f4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c9f4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8c9f4-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8c9f4-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8c9f4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c9f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c9f4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c9f4-116">Not supported.</span></span>    |
|<span data-ttu-id="8c9f4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c9f4-117">Application</span></span> | <span data-ttu-id="8c9f4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c9f4-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c9f4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c9f4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="8c9f4-120">Observe que ``<id>`` está no formato de 'userId_roleId', onde userId é a cadeia de caracteres do GUID para id de usuário do Windows Azure AD e roleId é a cadeia de caracteres do GUID para id de função de administrador do Azure.</span><span class="sxs-lookup"><span data-stu-id="8c9f4-120">Note that ``<id>`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c9f4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c9f4-121">Request headers</span></span>
| <span data-ttu-id="8c9f4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8c9f4-122">Name</span></span>       | <span data-ttu-id="8c9f4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c9f4-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8c9f4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c9f4-124">Authorization</span></span>  | <span data-ttu-id="8c9f4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c9f4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c9f4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c9f4-127">Request body</span></span>
<span data-ttu-id="8c9f4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8c9f4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c9f4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c9f4-129">Response</span></span>

<span data-ttu-id="8c9f4-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c9f4-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="8c9f4-132">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="8c9f4-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="8c9f4-133">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="8c9f4-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="8c9f4-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c9f4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c9f4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c9f4-135">Request</span></span>
<span data-ttu-id="8c9f4-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c9f4-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="8c9f4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c9f4-137">Response</span></span>
<span data-ttu-id="8c9f4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c9f4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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