---
title: Lista de configurações de grupo
description: Recuperar uma lista de objetos de configuração de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8cb245c786ef1fbede3e305fd73df74eb574393c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932361"
---
# <a name="list-group-settings"></a><span data-ttu-id="61625-103">Lista de configurações de grupo</span><span class="sxs-lookup"><span data-stu-id="61625-103">List group settings</span></span>

<span data-ttu-id="61625-104">Recuperar uma lista de objetos de configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="61625-104">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="61625-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="61625-105">Permissions</span></span>

<span data-ttu-id="61625-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61625-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="61625-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61625-108">Permission type</span></span>      | <span data-ttu-id="61625-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61625-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61625-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61625-110">Delegated (work or school account)</span></span> | <span data-ttu-id="61625-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="61625-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="61625-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61625-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61625-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61625-113">Not supported.</span></span>    |
|<span data-ttu-id="61625-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61625-114">Application</span></span> | <span data-ttu-id="61625-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61625-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61625-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61625-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="61625-117">Lista configurações de todo o locatário ou específico.</span><span class="sxs-lookup"><span data-stu-id="61625-117">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="61625-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="61625-118">Optional query parameters</span></span>
<span data-ttu-id="61625-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="61625-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="61625-120">Observação: $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="61625-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61625-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61625-121">Request headers</span></span>
| <span data-ttu-id="61625-122">Nome</span><span class="sxs-lookup"><span data-stu-id="61625-122">Name</span></span> | <span data-ttu-id="61625-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="61625-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="61625-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="61625-124">Authorization</span></span>  | <span data-ttu-id="61625-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61625-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61625-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61625-127">Request body</span></span>
<span data-ttu-id="61625-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61625-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61625-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="61625-129">Response</span></span>

<span data-ttu-id="61625-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61625-130">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="61625-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61625-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="61625-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61625-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
##### <a name="response"></a><span data-ttu-id="61625-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="61625-133">Response</span></span>

<span data-ttu-id="61625-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61625-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "displayName": "displayName-value",
      "templateId": "templateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ],
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
