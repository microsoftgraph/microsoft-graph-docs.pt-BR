---
title: Lista de configurações de grupo
description: Recuperar uma lista de objetos de configuração de grupo.
ms.openlocfilehash: 2a34627f057a5244a94d7f9e14dde5df1fe12202
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005331"
---
# <a name="list-group-settings"></a><span data-ttu-id="09d67-103">Lista de configurações de grupo</span><span class="sxs-lookup"><span data-stu-id="09d67-103">List group settings</span></span>

<span data-ttu-id="09d67-104">Recuperar uma lista de objetos de configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="09d67-104">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="09d67-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="09d67-105">Permissions</span></span>

<span data-ttu-id="09d67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09d67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="09d67-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09d67-108">Permission type</span></span>      | <span data-ttu-id="09d67-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09d67-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09d67-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09d67-110">Delegated (work or school account)</span></span> | <span data-ttu-id="09d67-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09d67-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="09d67-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09d67-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09d67-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09d67-113">Not supported.</span></span>    |
|<span data-ttu-id="09d67-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09d67-114">Application</span></span> | <span data-ttu-id="09d67-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09d67-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09d67-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09d67-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="09d67-117">Lista configurações de todo o locatário ou específico.</span><span class="sxs-lookup"><span data-stu-id="09d67-117">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="09d67-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="09d67-118">Optional query parameters</span></span>
<span data-ttu-id="09d67-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="09d67-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="09d67-120">Observação: $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="09d67-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09d67-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09d67-121">Request headers</span></span>
| <span data-ttu-id="09d67-122">Nome</span><span class="sxs-lookup"><span data-stu-id="09d67-122">Name</span></span> | <span data-ttu-id="09d67-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="09d67-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="09d67-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="09d67-124">Authorization</span></span>  | <span data-ttu-id="09d67-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09d67-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09d67-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09d67-127">Request body</span></span>
<span data-ttu-id="09d67-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09d67-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09d67-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="09d67-129">Response</span></span>

<span data-ttu-id="09d67-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09d67-130">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09d67-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09d67-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="09d67-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09d67-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
##### <a name="response"></a><span data-ttu-id="09d67-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="09d67-133">Response</span></span>

<span data-ttu-id="09d67-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09d67-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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