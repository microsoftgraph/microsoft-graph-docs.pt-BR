---
title: 'directoryObject: getAvailableExtensionProperties'
description: Obtenha todas as listas ou uma lista filtrada das propriedades de extensão do diretório que foram registradas em um diretório.
author: sureshja
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0464228669013360ad71eb24d214c4810bdb4c43
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434409"
---
# <a name="directoryobject-getavailableextensionproperties"></a><span data-ttu-id="2d7b8-103">directoryObject: getAvailableExtensionProperties</span><span class="sxs-lookup"><span data-stu-id="2d7b8-103">directoryObject: getAvailableExtensionProperties</span></span>
<span data-ttu-id="2d7b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d7b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d7b8-105">Retorne todas ou uma lista filtrada das propriedades de extensão de diretório que foram registradas em um diretório.</span><span class="sxs-lookup"><span data-stu-id="2d7b8-105">Return all or a filtered list of the directory extension properties that have been registered in a directory.</span></span> <span data-ttu-id="2d7b8-106">As entidades a seguir suportam propriedades de extensão: **usuário**, **grupo** **,** organização , **dispositivo,** **aplicativo** e **servicePrincipal**.</span><span class="sxs-lookup"><span data-stu-id="2d7b8-106">The following entities support extension properties: **user**, **group**, **organization**, **device**, **application**, and **servicePrincipal**.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d7b8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2d7b8-107">Permissions</span></span>
<span data-ttu-id="2d7b8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d7b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d7b8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d7b8-110">Permission type</span></span>|<span data-ttu-id="2d7b8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d7b8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d7b8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d7b8-112">Delegated (work or school account)</span></span>| <span data-ttu-id="2d7b8-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d7b8-113">Directory.Read.All</span></span> |
|<span data-ttu-id="2d7b8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d7b8-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="2d7b8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d7b8-115">Not supported.</span></span> |
|<span data-ttu-id="2d7b8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d7b8-116">Application</span></span>| <span data-ttu-id="2d7b8-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d7b8-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d7b8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d7b8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /directoryObjects/getAvailableExtensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="2d7b8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d7b8-119">Request headers</span></span>
|<span data-ttu-id="2d7b8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2d7b8-120">Name</span></span>|<span data-ttu-id="2d7b8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d7b8-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2d7b8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d7b8-122">Authorization</span></span>|<span data-ttu-id="2d7b8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d7b8-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2d7b8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d7b8-125">Content-Type</span></span>|<span data-ttu-id="2d7b8-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d7b8-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d7b8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d7b8-128">Request body</span></span>
<span data-ttu-id="2d7b8-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="2d7b8-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2d7b8-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="2d7b8-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2d7b8-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2d7b8-131">Parameter</span></span>|<span data-ttu-id="2d7b8-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d7b8-132">Type</span></span>|<span data-ttu-id="2d7b8-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d7b8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d7b8-134">isSyncedFromOnPremises</span><span class="sxs-lookup"><span data-stu-id="2d7b8-134">isSyncedFromOnPremises</span></span>|<span data-ttu-id="2d7b8-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d7b8-135">Boolean</span></span>|<span data-ttu-id="2d7b8-136">`true` para especificar que apenas as propriedades de extensão sincronizadas do diretório local devem ser retornadas; para especificar que apenas as propriedades de extensão que não são sincronizadas do diretório `false` local devem ser retornadas.</span><span class="sxs-lookup"><span data-stu-id="2d7b8-136">`true` to specify that only extension properties that are synced from the on-premises directory should be returned; `false` to specify that only extension properties that are not synced from the on-premises directory should be returned.</span></span> <span data-ttu-id="2d7b8-137">Se o parâmetro for omitido, todas as propriedades de extensão (sincronizadas e não sincronizadas) serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="2d7b8-137">If the parameter is omitted, all extension properties (both synced and non-synced) are returned.</span></span>|


## <a name="response"></a><span data-ttu-id="2d7b8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d7b8-138">Response</span></span>

<span data-ttu-id="2d7b8-139">Se tiver êxito, essa ação retornará um código de resposta e uma coleção `200 OK` [extensionProperty](../resources/extensionproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d7b8-139">If successful, this action returns a `200 OK` response code and an [extensionProperty](../resources/extensionproperty.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d7b8-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2d7b8-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d7b8-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d7b8-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2d7b8-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d7b8-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getavailableextensionproperties"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/directoryObjects/getAvailableExtensionProperties
Content-Type: application/json
Content-length: 43

{
  "isSyncedFromOnPremises": "Boolean"
}
```
# <a name="javascript"></a>[<span data-ttu-id="2d7b8-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d7b8-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getavailableextensionproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="2d7b8-144">C#</span><span class="sxs-lookup"><span data-stu-id="2d7b8-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getavailableextensionproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d7b8-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d7b8-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getavailableextensionproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d7b8-146">Java</span><span class="sxs-lookup"><span data-stu-id="2d7b8-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getavailableextensionproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2d7b8-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d7b8-147">Response</span></span>
> <span data-ttu-id="2d7b8-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2d7b8-148">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.extensionProperty)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.extensionProperty",
      "id": "d6a8bfec-893d-46e4-88fd-7db5fcc0fa62",
      "deletedDateTime": null,
      "appDisplayName": "SampleApp",
      "name": "extension_4d405aa8baa04fb494d3e0571fd9fd71_skypeId",
      "dataType": "String",
      "isSyncedFromOnPremises": false,
      "targetObjects": [
        "User"
      ]
    }
  ]
}
```


