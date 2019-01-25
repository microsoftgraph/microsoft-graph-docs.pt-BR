---
title: Configurações do diretório de lista
description: Recupere uma lista de objetos de configuração do diretório.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 708faad9dc90bf5f79f89d72b381391843371766
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515934"
---
# <a name="list-directory-settings"></a><span data-ttu-id="32648-103">Configurações do diretório de lista</span><span class="sxs-lookup"><span data-stu-id="32648-103">List directory settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32648-104">Recupere uma lista de objetos de configuração do diretório.</span><span class="sxs-lookup"><span data-stu-id="32648-104">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="32648-105">**Observação**: A versão de /beta desse API é só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="32648-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="32648-106">A versão de /v1.0 desse API foi renomeada para *groupSettings de lista*.</span><span class="sxs-lookup"><span data-stu-id="32648-106">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="32648-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="32648-107">Permissions</span></span>
<span data-ttu-id="32648-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32648-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32648-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32648-110">Permission type</span></span>      | <span data-ttu-id="32648-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32648-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32648-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32648-112">Delegated (work or school account)</span></span> | <span data-ttu-id="32648-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="32648-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="32648-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32648-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32648-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32648-115">Not supported.</span></span>    |
|<span data-ttu-id="32648-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32648-116">Application</span></span> | <span data-ttu-id="32648-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32648-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32648-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32648-118">HTTP request</span></span>
<span data-ttu-id="32648-119"><!-- { "blockType": "ignored" } -->Listar todo o locatário ou configurações de grupo</span><span class="sxs-lookup"><span data-stu-id="32648-119"><!-- { "blockType": "ignored" } --> List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="32648-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="32648-120">Optional query parameters</span></span>
<span data-ttu-id="32648-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="32648-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32648-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32648-122">Request headers</span></span>
| <span data-ttu-id="32648-123">Nome</span><span class="sxs-lookup"><span data-stu-id="32648-123">Name</span></span>      |<span data-ttu-id="32648-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="32648-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="32648-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="32648-125">Authorization</span></span>  | <span data-ttu-id="32648-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32648-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32648-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32648-128">Request body</span></span>
<span data-ttu-id="32648-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32648-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32648-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="32648-130">Response</span></span>

<span data-ttu-id="32648-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32648-131">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="32648-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32648-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32648-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32648-133">Request</span></span>
<span data-ttu-id="32648-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32648-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
##### <a name="response"></a><span data-ttu-id="32648-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="32648-135">Response</span></span>
<span data-ttu-id="32648-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32648-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "id": "id-value",
      "displayName": "displayName-value",
      "settingTemplateId": "settingTemplateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
