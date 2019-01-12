---
title: Obter objetos directory a partir de uma lista de ids
description: Selecione ' opção de consulta não está disponível para esta operação.
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2fab85844d810627ca4e44395477716eb0828ffa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986814"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="56254-103">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="56254-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="56254-p101">Retorna os objetos directory especificados a partir de uma lista de ids  OBSERVAÇÃO: Os objetos de diretório retornados são os objetos completos que contêm **todas** as propriedades. A opção `$select` não está disponível para todos os tipos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="56254-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="56254-107">Alguns usos comuns dessa função são:</span><span class="sxs-lookup"><span data-stu-id="56254-107">Some common uses for this function are to:</span></span>

* <span data-ttu-id="56254-108">Resolver ids retornadas por funções (que retornam coleções de ids) como [getMemberObjects](directoryobject-getmemberobjects.md) ou [getMemberGroups](directoryobject-getmembergroups.md) para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="56254-108">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="56254-109">Resolver ids que persistem em um repositório externo pelo aplicativo para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="56254-109">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="56254-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="56254-110">Permissions</span></span>

<span data-ttu-id="56254-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56254-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="56254-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56254-113">Permission type</span></span>      | <span data-ttu-id="56254-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56254-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56254-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56254-115">Delegated (work or school account)</span></span> | <span data-ttu-id="56254-116">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="56254-116">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="56254-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56254-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56254-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56254-118">Not supported.</span></span>    |
|<span data-ttu-id="56254-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56254-119">Application</span></span> | <span data-ttu-id="56254-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="56254-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56254-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56254-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="56254-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56254-122">Request headers</span></span>

| <span data-ttu-id="56254-123">Nome</span><span class="sxs-lookup"><span data-stu-id="56254-123">Name</span></span>       | <span data-ttu-id="56254-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="56254-124">Type</span></span> | <span data-ttu-id="56254-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="56254-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="56254-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="56254-126">Authorization</span></span>  | <span data-ttu-id="56254-127">string</span><span class="sxs-lookup"><span data-stu-id="56254-127">string</span></span>  | <span data-ttu-id="56254-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56254-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56254-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56254-130">Content-Type</span></span>  | <span data-ttu-id="56254-131">string</span><span class="sxs-lookup"><span data-stu-id="56254-131">string</span></span> | <span data-ttu-id="56254-132">application/json</span><span class="sxs-lookup"><span data-stu-id="56254-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="56254-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56254-133">Request body</span></span>

<span data-ttu-id="56254-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56254-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="56254-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="56254-135">Parameter</span></span>   | <span data-ttu-id="56254-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="56254-136">Type</span></span> |<span data-ttu-id="56254-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="56254-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56254-138">ids</span><span class="sxs-lookup"><span data-stu-id="56254-138">ids</span></span>|<span data-ttu-id="56254-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="56254-139">String collection</span></span>| <span data-ttu-id="56254-p104">Uma coleção de ids para a qual retornar objetos. Você pode especificar até 1000 ids.</span><span class="sxs-lookup"><span data-stu-id="56254-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="56254-142">tipos</span><span class="sxs-lookup"><span data-stu-id="56254-142">types</span></span>|<span data-ttu-id="56254-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="56254-143">String collection</span></span>| <span data-ttu-id="56254-144">Uma coleção dos tipos de recursos que especifica o conjunto de conjuntos de recursos para pesquisar.</span><span class="sxs-lookup"><span data-stu-id="56254-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="56254-145">Se não especificado, o padrão é [directoryObject](../resources/directoryobject.md), que contém todos os tipos de recursos definidos no diretório.</span><span class="sxs-lookup"><span data-stu-id="56254-145">If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="56254-146">Qualquer objeto que derive da `directoryObject` podem ser especificados na coleção; Por exemplo: [usuário](../resources/user.md), [grupo](../resources/group.md), [dispositivo](../resources/device.md)e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="56254-146">Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on.</span></span> <span data-ttu-id="56254-147">Os valores não diferenciam maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="56254-147">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="56254-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="56254-148">Response</span></span>

<span data-ttu-id="56254-149">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56254-149">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56254-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56254-150">Example</span></span>

##### <a name="request"></a><span data-ttu-id="56254-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56254-151">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="56254-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="56254-152">Response</span></span>

<span data-ttu-id="56254-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56254-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
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
