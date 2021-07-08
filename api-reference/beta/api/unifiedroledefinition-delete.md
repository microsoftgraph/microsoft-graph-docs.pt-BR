---
title: Excluir unifiedRoleDefinition
description: Exclua um objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7de16492df085b48d2fe580ff54d3cacf9dc0d22
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334364"
---
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="18339-103">Excluir unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="18339-103">Delete unifiedRoleDefinition</span></span>

<span data-ttu-id="18339-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18339-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18339-105">[Exclua um objeto unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) para um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="18339-105">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="18339-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="18339-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="18339-107">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="18339-107">device management (Intune)</span></span>
- <span data-ttu-id="18339-108">directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="18339-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="18339-109">No momento, o provedor RBAC do computador na nuvem dá suporte apenas à [lista](rbacapplication-list-roledefinitions.md) e [obter](unifiedroledefinition-get.md) operações.</span><span class="sxs-lookup"><span data-stu-id="18339-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="18339-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="18339-110">Permissions</span></span>

<span data-ttu-id="18339-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="18339-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="18339-112">Para saber mais, incluindo [ter cuidado antes](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) de escolher permissões mais privilegiadas, consulte [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18339-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="18339-113">Para o provedor de gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="18339-113">For Device management (Intune) provider</span></span>

|<span data-ttu-id="18339-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18339-114">Permission type</span></span>      | <span data-ttu-id="18339-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18339-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18339-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18339-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="18339-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18339-117">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="18339-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18339-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18339-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18339-119">Not supported.</span></span>    |
|<span data-ttu-id="18339-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18339-120">Application</span></span> | <span data-ttu-id="18339-121">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18339-121">DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="18339-122">Provedor do Azure AD (Diretório)</span><span class="sxs-lookup"><span data-stu-id="18339-122">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="18339-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18339-123">Permission type</span></span>      | <span data-ttu-id="18339-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18339-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18339-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18339-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="18339-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18339-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="18339-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18339-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18339-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18339-128">Not supported.</span></span>    |
|<span data-ttu-id="18339-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18339-129">Application</span></span> | <span data-ttu-id="18339-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18339-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18339-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18339-131">HTTP request</span></span>

<span data-ttu-id="18339-132">Para excluir uma definição de função para um provedor de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="18339-132">To delete a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="18339-133">Para excluir uma definição de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="18339-133">To delete a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="18339-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18339-134">Request headers</span></span>

| <span data-ttu-id="18339-135">Nome</span><span class="sxs-lookup"><span data-stu-id="18339-135">Name</span></span>          | <span data-ttu-id="18339-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="18339-136">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="18339-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="18339-137">Authorization</span></span> | <span data-ttu-id="18339-138">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="18339-138">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="18339-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18339-139">Request body</span></span>

<span data-ttu-id="18339-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="18339-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18339-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="18339-141">Response</span></span>

<span data-ttu-id="18339-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18339-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18339-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18339-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="18339-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18339-145">Request</span></span>

<span data-ttu-id="18339-146">O exemplo a seguir exclui um **unifiedRoleDefinition para** um provedor de diretórios.</span><span class="sxs-lookup"><span data-stu-id="18339-146">The following example deletes a **unifiedRoleDefinition** for a directory provider.</span></span>

# <a name="http"></a>[<span data-ttu-id="18339-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="18339-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="18339-148">C#</span><span class="sxs-lookup"><span data-stu-id="18339-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18339-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18339-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18339-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18339-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18339-151">Java</span><span class="sxs-lookup"><span data-stu-id="18339-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18339-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="18339-152">Response</span></span>

<span data-ttu-id="18339-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18339-153">The following is an example of the response.</span></span>

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


