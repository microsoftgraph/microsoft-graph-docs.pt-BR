---
title: Fazer uma configuração de diretório
description: Recupere as propriedades de um objeto de configuração do diretório específico.
author: lleonard-msft
ms.openlocfilehash: 7dfd6d7f7623aef082a43c0b67c1867edb691f31
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361471"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="ee901-103">Fazer uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="ee901-103">Get a directory setting</span></span>

> <span data-ttu-id="ee901-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ee901-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee901-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ee901-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ee901-106">Recupere as propriedades de um objeto de configuração do diretório específico.</span><span class="sxs-lookup"><span data-stu-id="ee901-106">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="ee901-107">**Observação**: A versão de /beta desse API é só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="ee901-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="ee901-108">A versão de /v1.0 desse API foi renomeada para *obter groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="ee901-108">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee901-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee901-109">Permissions</span></span>
<span data-ttu-id="ee901-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee901-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee901-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee901-112">Permission type</span></span>      | <span data-ttu-id="ee901-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee901-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee901-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee901-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ee901-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee901-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee901-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee901-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee901-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee901-117">Not supported.</span></span>    |
|<span data-ttu-id="ee901-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee901-118">Application</span></span> | <span data-ttu-id="ee901-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee901-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee901-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee901-120">HTTP request</span></span>
<span data-ttu-id="ee901-121"><!-- { "blockType": "ignored" } -->Obter um locatário todo específico ou configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="ee901-121"><!-- { "blockType": "ignored" } --> Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ee901-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ee901-122">Optional query parameters</span></span>
<span data-ttu-id="ee901-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ee901-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee901-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee901-124">Request headers</span></span>
| <span data-ttu-id="ee901-125">Nome</span><span class="sxs-lookup"><span data-stu-id="ee901-125">Name</span></span>      |<span data-ttu-id="ee901-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee901-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ee901-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee901-127">Authorization</span></span>  | <span data-ttu-id="ee901-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee901-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee901-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee901-130">Request body</span></span>
<span data-ttu-id="ee901-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee901-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee901-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee901-132">Response</span></span>

<span data-ttu-id="ee901-133">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee901-133">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ee901-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee901-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee901-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee901-135">Request</span></span>
<span data-ttu-id="ee901-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee901-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="ee901-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee901-137">Response</span></span>
<span data-ttu-id="ee901-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee901-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 198

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->