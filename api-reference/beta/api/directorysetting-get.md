---
title: Fazer uma configuração de diretório
description: Recupere as propriedades de um objeto de configuração do diretório específico.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 73953ccedeb7ecaeeba5cb68e6827956430ada82
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950820"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="3a4d4-103">Fazer uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="3a4d4-103">Get a directory setting</span></span>

> <span data-ttu-id="3a4d4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3a4d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a4d4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3a4d4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a4d4-106">Recupere as propriedades de um objeto de configuração do diretório específico.</span><span class="sxs-lookup"><span data-stu-id="3a4d4-106">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="3a4d4-107">**Observação**: A versão de /beta desse API é só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="3a4d4-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="3a4d4-108">A versão de /v1.0 desse API foi renomeada para *obter groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="3a4d4-108">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a4d4-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a4d4-109">Permissions</span></span>
<span data-ttu-id="3a4d4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a4d4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a4d4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a4d4-112">Permission type</span></span>      | <span data-ttu-id="3a4d4-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a4d4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a4d4-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a4d4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3a4d4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a4d4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3a4d4-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a4d4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a4d4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a4d4-117">Not supported.</span></span>    |
|<span data-ttu-id="3a4d4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a4d4-118">Application</span></span> | <span data-ttu-id="3a4d4-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a4d4-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a4d4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a4d4-120">HTTP request</span></span>
<span data-ttu-id="3a4d4-121"><!-- { "blockType": "ignored" } -->Obter um locatário todo específico ou configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="3a4d4-121"><!-- { "blockType": "ignored" } --> Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a4d4-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3a4d4-122">Optional query parameters</span></span>
<span data-ttu-id="3a4d4-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3a4d4-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a4d4-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a4d4-124">Request headers</span></span>
| <span data-ttu-id="3a4d4-125">Nome</span><span class="sxs-lookup"><span data-stu-id="3a4d4-125">Name</span></span>      |<span data-ttu-id="3a4d4-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a4d4-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3a4d4-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a4d4-127">Authorization</span></span>  | <span data-ttu-id="3a4d4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a4d4-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a4d4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a4d4-130">Request body</span></span>
<span data-ttu-id="3a4d4-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a4d4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a4d4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a4d4-132">Response</span></span>

<span data-ttu-id="3a4d4-133">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a4d4-133">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a4d4-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a4d4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a4d4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a4d4-135">Request</span></span>
<span data-ttu-id="3a4d4-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a4d4-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="3a4d4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a4d4-137">Response</span></span>
<span data-ttu-id="3a4d4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a4d4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
