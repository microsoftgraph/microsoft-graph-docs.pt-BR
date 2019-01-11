---
title: 'servicePrincipals: listar ownedObjects'
description: Recupere uma lista de objetos pertencentes a servicePrincipal.  Isso pode incluir aplicativos ou grupos.
localization_priority: Normal
ms.openlocfilehash: f061a99c6389651985779ac71df2ced5a91ba527
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882863"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="93226-104">servicePrincipals: listar ownedObjects</span><span class="sxs-lookup"><span data-stu-id="93226-104">servicePrincipals: List ownedObjects</span></span>

> <span data-ttu-id="93226-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="93226-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93226-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="93226-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93226-107">Recupere uma lista de objetos pertencentes a servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="93226-107">Retrieve a list of objects owned by the servicePrincipal.</span></span>  <span data-ttu-id="93226-108">Isso pode incluir aplicativos ou grupos.</span><span class="sxs-lookup"><span data-stu-id="93226-108">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="93226-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="93226-109">Permissions</span></span>
<span data-ttu-id="93226-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93226-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93226-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93226-112">Permission type</span></span>      | <span data-ttu-id="93226-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93226-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93226-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93226-114">Delegated (work or school account)</span></span> | <span data-ttu-id="93226-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="93226-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="93226-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93226-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93226-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93226-117">Not supported.</span></span>    |
|<span data-ttu-id="93226-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93226-118">Application</span></span> | <span data-ttu-id="93226-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93226-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93226-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93226-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="93226-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="93226-121">Optional query parameters</span></span>
<span data-ttu-id="93226-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="93226-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93226-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93226-123">Request headers</span></span>
| <span data-ttu-id="93226-124">Nome</span><span class="sxs-lookup"><span data-stu-id="93226-124">Name</span></span>       | <span data-ttu-id="93226-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="93226-125">Type</span></span> | <span data-ttu-id="93226-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="93226-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="93226-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="93226-127">Authorization</span></span>  | <span data-ttu-id="93226-128">string</span><span class="sxs-lookup"><span data-stu-id="93226-128">string</span></span>  | <span data-ttu-id="93226-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93226-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93226-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93226-131">Request body</span></span>
<span data-ttu-id="93226-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93226-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93226-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="93226-133">Response</span></span>

<span data-ttu-id="93226-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93226-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93226-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93226-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93226-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93226-136">Request</span></span>
<span data-ttu-id="93226-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93226-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
##### <a name="response"></a><span data-ttu-id="93226-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="93226-138">Response</span></span>
<span data-ttu-id="93226-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93226-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
