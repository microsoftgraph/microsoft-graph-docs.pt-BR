---
title: Obter objetos directory a partir de uma lista de ids
description: Selecione ' opção de consulta não está disponível para esta operação.
ms.openlocfilehash: 87fa774910c1ea6795b6df65ee0f5538d12296bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034066"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="1f8e0-103">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="1f8e0-103">Get directory objects from a list of ids</span></span>

> <span data-ttu-id="1f8e0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f8e0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f8e0-p102">Retorna os objetos directory especificados a partir de uma lista de ids  OBSERVAÇÃO: Os objetos de diretório retornados são os objetos completos que contêm **todas** as propriedades. A opção `$select` não está disponível para todos os tipos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-p102">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="1f8e0-109">Alguns usos comuns dessa função são:</span><span class="sxs-lookup"><span data-stu-id="1f8e0-109">Some common uses for this function are to:</span></span>

* <span data-ttu-id="1f8e0-110">Resolver ids retornadas por funções (que retornam coleções de ids) como [getMemberObjects](directoryobject-getmemberobjects.md) ou [getMemberGroups](directoryobject-getmembergroups.md) para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-110">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="1f8e0-111">Resolver ids que persistem em um repositório externo pelo aplicativo para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-111">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f8e0-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f8e0-112">Permissions</span></span>

<span data-ttu-id="1f8e0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f8e0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1f8e0-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f8e0-115">Permission type</span></span>      | <span data-ttu-id="1f8e0-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f8e0-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f8e0-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f8e0-117">Delegated (work or school account)</span></span> | <span data-ttu-id="1f8e0-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f8e0-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="1f8e0-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f8e0-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f8e0-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-120">Not supported.</span></span>    |
|<span data-ttu-id="1f8e0-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f8e0-121">Application</span></span> | <span data-ttu-id="1f8e0-122">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f8e0-122">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f8e0-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f8e0-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getById
```

## <a name="request-headers"></a><span data-ttu-id="1f8e0-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f8e0-124">Request headers</span></span>

| <span data-ttu-id="1f8e0-125">Nome</span><span class="sxs-lookup"><span data-stu-id="1f8e0-125">Name</span></span>       | <span data-ttu-id="1f8e0-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f8e0-126">Type</span></span> | <span data-ttu-id="1f8e0-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f8e0-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1f8e0-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f8e0-128">Authorization</span></span>  | <span data-ttu-id="1f8e0-129">string</span><span class="sxs-lookup"><span data-stu-id="1f8e0-129">string</span></span>  | <span data-ttu-id="1f8e0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f8e0-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f8e0-132">Content-Type</span></span>  | <span data-ttu-id="1f8e0-133">application/json</span><span class="sxs-lookup"><span data-stu-id="1f8e0-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1f8e0-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f8e0-134">Request body</span></span>

<span data-ttu-id="1f8e0-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1f8e0-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1f8e0-136">Parameter</span></span>   | <span data-ttu-id="1f8e0-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f8e0-137">Type</span></span> |<span data-ttu-id="1f8e0-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f8e0-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f8e0-139">ids</span><span class="sxs-lookup"><span data-stu-id="1f8e0-139">ids</span></span>|<span data-ttu-id="1f8e0-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f8e0-140">String collection</span></span>| <span data-ttu-id="1f8e0-p105">Uma coleção de ids para a qual retornar objetos. Você pode especificar até 1000 ids.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-p105">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="1f8e0-143">tipos</span><span class="sxs-lookup"><span data-stu-id="1f8e0-143">types</span></span>|<span data-ttu-id="1f8e0-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f8e0-144">String collection</span></span>| <span data-ttu-id="1f8e0-145">Uma coleção dos tipos de recursos que especifica o conjunto de conjuntos de recursos para pesquisar.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-145">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="1f8e0-146">Se não especificado, o padrão é [directoryObject](../resources/directoryobject.md), que contém todos os tipos de recursos definidos no diretório.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-146">If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="1f8e0-147">Qualquer objeto que derive da `directoryObject` podem ser especificados na coleção; Por exemplo: [usuário](../resources/user.md), [grupo](../resources/group.md), [dispositivo](../resources/device.md)e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-147">Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on.</span></span> <span data-ttu-id="1f8e0-148">Os valores não diferenciam maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-148">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="1f8e0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f8e0-149">Response</span></span>

<span data-ttu-id="1f8e0-150">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-150">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f8e0-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f8e0-151">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1f8e0-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f8e0-152">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/beta/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="1f8e0-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f8e0-153">Response</span></span>

<span data-ttu-id="1f8e0-p107">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f8e0-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
