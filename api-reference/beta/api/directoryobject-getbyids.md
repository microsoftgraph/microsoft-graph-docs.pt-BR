---
title: Obter objetos directory a partir de uma lista de ids
description: Selecione ' opção de consulta não está disponível para esta operação.
author: lleonard-msft
ms.openlocfilehash: 335a6ba915e714ebbd95ba818d14043037f38050
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336285"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="64b7a-103">Obter objetos directory a partir de uma lista de ids</span><span class="sxs-lookup"><span data-stu-id="64b7a-103">Get directory objects from a list of ids</span></span>

> <span data-ttu-id="64b7a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="64b7a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64b7a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="64b7a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64b7a-p102">Retorna os objetos directory especificados a partir de uma lista de ids  OBSERVAÇÃO: Os objetos de diretório retornados são os objetos completos que contêm **todas** as propriedades. A opção `$select` não está disponível para todos os tipos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="64b7a-p102">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="64b7a-109">Alguns usos comuns dessa função são:</span><span class="sxs-lookup"><span data-stu-id="64b7a-109">Some common uses for this function are to:</span></span>

* <span data-ttu-id="64b7a-110">Resolver ids retornadas por funções (que retornam coleções de ids) como [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) ou [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta) para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="64b7a-110">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) or [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)  to their backing directory objects.</span></span>
* <span data-ttu-id="64b7a-111">Resolver ids que persistem em um repositório externo pelo aplicativo para seus objetos de diretório de suporte.</span><span class="sxs-lookup"><span data-stu-id="64b7a-111">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="64b7a-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="64b7a-112">Permissions</span></span>

<span data-ttu-id="64b7a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64b7a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="64b7a-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64b7a-115">Permission type</span></span>      | <span data-ttu-id="64b7a-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64b7a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64b7a-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64b7a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="64b7a-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="64b7a-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="64b7a-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64b7a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64b7a-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64b7a-120">Not supported.</span></span>    |
|<span data-ttu-id="64b7a-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64b7a-121">Application</span></span> | <span data-ttu-id="64b7a-122">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="64b7a-122">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64b7a-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64b7a-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="64b7a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64b7a-124">Request headers</span></span>

| <span data-ttu-id="64b7a-125">Nome</span><span class="sxs-lookup"><span data-stu-id="64b7a-125">Name</span></span>       | <span data-ttu-id="64b7a-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="64b7a-126">Type</span></span> | <span data-ttu-id="64b7a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="64b7a-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="64b7a-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="64b7a-128">Authorization</span></span>  | <span data-ttu-id="64b7a-129">string</span><span class="sxs-lookup"><span data-stu-id="64b7a-129">string</span></span>  | <span data-ttu-id="64b7a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64b7a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64b7a-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64b7a-132">Content-Type</span></span>  | <span data-ttu-id="64b7a-133">application/json</span><span class="sxs-lookup"><span data-stu-id="64b7a-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64b7a-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64b7a-134">Request body</span></span>

<span data-ttu-id="64b7a-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64b7a-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="64b7a-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="64b7a-136">Parameter</span></span>   | <span data-ttu-id="64b7a-137">Type</span><span class="sxs-lookup"><span data-stu-id="64b7a-137">Type</span></span> |<span data-ttu-id="64b7a-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="64b7a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64b7a-139">ids</span><span class="sxs-lookup"><span data-stu-id="64b7a-139">ids</span></span>|<span data-ttu-id="64b7a-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="64b7a-140">String collection</span></span>| <span data-ttu-id="64b7a-p105">Uma coleção de ids para a qual retornar objetos. Você pode especificar até 1000 ids.</span><span class="sxs-lookup"><span data-stu-id="64b7a-p105">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="64b7a-143">tipos</span><span class="sxs-lookup"><span data-stu-id="64b7a-143">types</span></span>|<span data-ttu-id="64b7a-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="64b7a-144">String collection</span></span>| <span data-ttu-id="64b7a-145">Uma coleção dos tipos de recursos que especifica o conjunto de conjuntos de recursos para pesquisar.</span><span class="sxs-lookup"><span data-stu-id="64b7a-145">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="64b7a-146">Se não especificado, o padrão é [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), que contém todos os tipos de recursos definidos no diretório.</span><span class="sxs-lookup"><span data-stu-id="64b7a-146">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="64b7a-147">Qualquer objeto que derive da [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) pode ser especificado na coleção; Por exemplo: [usuário](/graph/api/resources/user?view=graph-rest-beta), [grupo](/graph/api/resources/group?view=graph-rest-beta), [dispositivo](/graph/api/resources/device?view=graph-rest-beta)e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="64b7a-147">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="64b7a-148">Para pesquisar referências a um parceiro de [Provedor de soluções de nuvem](https://partner.microsoft.com/en-us/cloud-solution-provider) organização especificar [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="64b7a-148">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="64b7a-149">Se não especificado, o padrão é [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), que contém todos os tipos de recursos definidos no diretório, exceto para referências a uma organização parceira de [Provedor de soluções de nuvem](https://partner.microsoft.com/en-us/cloud-solution-provider) .</span><span class="sxs-lookup"><span data-stu-id="64b7a-149">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="64b7a-150">Os valores não diferenciam maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="64b7a-150">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="64b7a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="64b7a-151">Response</span></span>

<span data-ttu-id="64b7a-152">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64b7a-152">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64b7a-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64b7a-153">Example</span></span>

##### <a name="request"></a><span data-ttu-id="64b7a-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64b7a-154">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getByIds"
}-->

```http
POST https://graph.microsoft.com/beta/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="64b7a-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="64b7a-155">Response</span></span>

<span data-ttu-id="64b7a-p107">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64b7a-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
