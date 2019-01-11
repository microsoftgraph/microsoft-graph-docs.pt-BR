---
title: Configurações do diretório de lista
description: Recupere uma lista de objetos de configuração do diretório.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 73756c81f19643fedcec0faa5f43125a7c389b35
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833401"
---
# <a name="list-directory-settings"></a><span data-ttu-id="2fdfe-103">Configurações do diretório de lista</span><span class="sxs-lookup"><span data-stu-id="2fdfe-103">List directory settings</span></span>

> <span data-ttu-id="2fdfe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2fdfe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fdfe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2fdfe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2fdfe-106">Recupere uma lista de objetos de configuração do diretório.</span><span class="sxs-lookup"><span data-stu-id="2fdfe-106">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="2fdfe-107">**Observação**: A versão de /beta desse API é só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="2fdfe-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="2fdfe-108">A versão de /v1.0 desse API foi renomeada para *groupSettings de lista*.</span><span class="sxs-lookup"><span data-stu-id="2fdfe-108">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fdfe-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="2fdfe-109">Permissions</span></span>
<span data-ttu-id="2fdfe-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fdfe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fdfe-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fdfe-112">Permission type</span></span>      | <span data-ttu-id="2fdfe-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fdfe-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fdfe-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fdfe-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2fdfe-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2fdfe-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2fdfe-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fdfe-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fdfe-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fdfe-117">Not supported.</span></span>    |
|<span data-ttu-id="2fdfe-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fdfe-118">Application</span></span> | <span data-ttu-id="2fdfe-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fdfe-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fdfe-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fdfe-120">HTTP request</span></span>
<span data-ttu-id="2fdfe-121"><!-- { "blockType": "ignored" } -->Listar todo o locatário ou configurações de grupo</span><span class="sxs-lookup"><span data-stu-id="2fdfe-121"><!-- { "blockType": "ignored" } --> List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2fdfe-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2fdfe-122">Optional query parameters</span></span>
<span data-ttu-id="2fdfe-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2fdfe-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2fdfe-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fdfe-124">Request headers</span></span>
| <span data-ttu-id="2fdfe-125">Nome</span><span class="sxs-lookup"><span data-stu-id="2fdfe-125">Name</span></span>      |<span data-ttu-id="2fdfe-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fdfe-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2fdfe-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fdfe-127">Authorization</span></span>  | <span data-ttu-id="2fdfe-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fdfe-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fdfe-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fdfe-130">Request body</span></span>
<span data-ttu-id="2fdfe-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2fdfe-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fdfe-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fdfe-132">Response</span></span>

<span data-ttu-id="2fdfe-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fdfe-133">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2fdfe-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fdfe-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2fdfe-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fdfe-135">Request</span></span>
<span data-ttu-id="2fdfe-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fdfe-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
##### <a name="response"></a><span data-ttu-id="2fdfe-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fdfe-137">Response</span></span>
<span data-ttu-id="2fdfe-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fdfe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
