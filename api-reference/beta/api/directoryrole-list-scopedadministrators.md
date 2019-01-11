---
title: Lista scopedMembers para uma função de diretório
description: Recupere uma lista de objetos scopedRoleMembership para uma função de diretório.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: dbe294d2f55f7e4c0ee265aa180551e7078a5ab1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859210"
---
# <a name="list-scopedmembers-for-a-directory-role"></a><span data-ttu-id="558de-103">Lista scopedMembers para uma função de diretório</span><span class="sxs-lookup"><span data-stu-id="558de-103">List scopedMembers for a directory role</span></span>

> <span data-ttu-id="558de-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="558de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="558de-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="558de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="558de-106">Recupere uma lista de objetos [scopedRoleMembership](../resources/scopedrolemembership.md) para uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="558de-106">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) objects for a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="558de-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="558de-107">Permissions</span></span>
<span data-ttu-id="558de-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="558de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="558de-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="558de-110">Permission type</span></span>      | <span data-ttu-id="558de-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="558de-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="558de-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="558de-112">Delegated (work or school account)</span></span> | <span data-ttu-id="558de-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="558de-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="558de-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="558de-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="558de-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="558de-115">Not supported.</span></span>    |
|<span data-ttu-id="558de-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="558de-116">Application</span></span> | <span data-ttu-id="558de-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="558de-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="558de-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="558de-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{id}/scopedMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="558de-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="558de-119">Optional query parameters</span></span>
<span data-ttu-id="558de-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="558de-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="558de-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="558de-121">Request headers</span></span>
| <span data-ttu-id="558de-122">Nome</span><span class="sxs-lookup"><span data-stu-id="558de-122">Name</span></span>      |<span data-ttu-id="558de-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="558de-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="558de-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="558de-124">Authorization</span></span>  | <span data-ttu-id="558de-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="558de-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="558de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="558de-127">Request body</span></span>
<span data-ttu-id="558de-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="558de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="558de-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="558de-129">Response</span></span>

<span data-ttu-id="558de-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="558de-130">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="558de-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="558de-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="558de-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="558de-132">Request</span></span>
<span data-ttu-id="558de-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="558de-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/scopedMembers
```
##### <a name="response"></a><span data-ttu-id="558de-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="558de-134">Response</span></span>
<span data-ttu-id="558de-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="558de-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "id": "id-value",
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List scopedmembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
