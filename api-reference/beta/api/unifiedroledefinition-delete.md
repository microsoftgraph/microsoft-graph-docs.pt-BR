---
title: Excluir unifiedRoleDefinition
description: Exclua um objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e9f2d549cef274a536575a2671e454198dbb9f5f
ms.sourcegitcommit: 30903b12daf4cf2841524c57743889e23d11f85a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2021
ms.locfileid: "52709497"
---
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="f22c8-103">Excluir unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f22c8-103">Delete unifiedRoleDefinition</span></span>

<span data-ttu-id="f22c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f22c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f22c8-105">[Exclua um objeto unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) para um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="f22c8-105">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="f22c8-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="f22c8-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="f22c8-107">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="f22c8-107">device management (Intune)</span></span>
- <span data-ttu-id="f22c8-108">directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="f22c8-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="f22c8-109">No momento, o provedor RBAC do computador na nuvem dá suporte apenas à [lista](rbacapplication-list-roledefinitions.md) e [obter](unifiedroledefinition-get.md) operações.</span><span class="sxs-lookup"><span data-stu-id="f22c8-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="f22c8-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f22c8-110">Permissions</span></span>

<span data-ttu-id="f22c8-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f22c8-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="f22c8-112">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f22c8-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="f22c8-113">Provedor com suporte</span><span class="sxs-lookup"><span data-stu-id="f22c8-113">Supported provider</span></span>      | <span data-ttu-id="f22c8-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f22c8-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="f22c8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f22c8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f22c8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f22c8-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="f22c8-117">Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="f22c8-117">Device management</span></span> | <span data-ttu-id="f22c8-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f22c8-118">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="f22c8-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f22c8-119">Not supported.</span></span> | <span data-ttu-id="f22c8-120">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f22c8-120">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="f22c8-121">Diretório</span><span class="sxs-lookup"><span data-stu-id="f22c8-121">Directory</span></span> | <span data-ttu-id="f22c8-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f22c8-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="f22c8-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f22c8-123">Not supported.</span></span>| <span data-ttu-id="f22c8-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f22c8-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f22c8-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f22c8-125">HTTP request</span></span>

<span data-ttu-id="f22c8-126">Para excluir uma definição de função para um provedor de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="f22c8-126">To delete a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="f22c8-127">Para excluir uma definição de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="f22c8-127">To delete a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="f22c8-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f22c8-128">Request headers</span></span>

| <span data-ttu-id="f22c8-129">Nome</span><span class="sxs-lookup"><span data-stu-id="f22c8-129">Name</span></span>          | <span data-ttu-id="f22c8-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f22c8-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f22c8-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="f22c8-131">Authorization</span></span> | <span data-ttu-id="f22c8-132">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f22c8-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f22c8-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f22c8-133">Request body</span></span>

<span data-ttu-id="f22c8-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f22c8-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f22c8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f22c8-135">Response</span></span>

<span data-ttu-id="f22c8-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f22c8-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f22c8-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f22c8-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f22c8-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f22c8-139">Request</span></span>

<span data-ttu-id="f22c8-140">O exemplo a seguir exclui um **unifiedRoleDefinition para** um provedor de diretórios.</span><span class="sxs-lookup"><span data-stu-id="f22c8-140">The following example deletes a **unifiedRoleDefinition** for a directory provider.</span></span>

# <a name="http"></a>[<span data-ttu-id="f22c8-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="f22c8-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="f22c8-142">C#</span><span class="sxs-lookup"><span data-stu-id="f22c8-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f22c8-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f22c8-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f22c8-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f22c8-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f22c8-145">Java</span><span class="sxs-lookup"><span data-stu-id="f22c8-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f22c8-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f22c8-146">Response</span></span>

<span data-ttu-id="f22c8-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f22c8-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


