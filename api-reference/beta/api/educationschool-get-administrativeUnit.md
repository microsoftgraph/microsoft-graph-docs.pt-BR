---
title: Obter administrativeUnit
description: Recupere o diretório simples **administrativeUnit** que corresponde a essa **educationSchool**.
ms.openlocfilehash: 49ac05b44bc89f827091c3b846885a58cb7b8956
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037330"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="363da-103">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="363da-103">Get administrativeUnit</span></span>

> <span data-ttu-id="363da-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="363da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="363da-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="363da-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="363da-106">Recupere o diretório simples **administrativeUnit** que corresponde a essa **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="363da-106">Retrieve the simple directory **administrativeUnit** that corresponds to this **educationSchool**.</span></span>

><span data-ttu-id="363da-107">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="363da-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="363da-108">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="363da-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="363da-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="363da-109">Permissions</span></span>
<span data-ttu-id="363da-110">Uma combinação de permissões é obrigatória para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="363da-110">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="363da-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="363da-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="363da-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="363da-112">Permission type</span></span>      | <span data-ttu-id="363da-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="363da-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="363da-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="363da-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="363da-115">Uma de EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="363da-115">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="363da-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="363da-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="363da-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="363da-117">Not supported.</span></span>  |
|<span data-ttu-id="363da-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="363da-118">Application</span></span> | <span data-ttu-id="363da-119">EduRoster.Read.All, EduRoster.ReadWrite.All além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="363da-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="363da-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="363da-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/administrativeUnit
```
## <a name="request-headers"></a><span data-ttu-id="363da-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="363da-121">Request headers</span></span>
| <span data-ttu-id="363da-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="363da-122">Header</span></span>       | <span data-ttu-id="363da-123">Valor</span><span class="sxs-lookup"><span data-stu-id="363da-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="363da-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="363da-124">Authorization</span></span>  | <span data-ttu-id="363da-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="363da-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="363da-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="363da-127">Request body</span></span>
<span data-ttu-id="363da-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="363da-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="363da-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="363da-129">Response</span></span>
<span data-ttu-id="363da-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="363da-130">If successful, this method returns a `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="363da-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="363da-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="363da-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="363da-132">Request</span></span>
<span data-ttu-id="363da-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="363da-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeUnit"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/2961761D-8094-4183-A9F6-8E36E966C7D9/administrativeUnit
```
##### <a name="response"></a><span data-ttu-id="363da-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="363da-134">Response</span></span>
<span data-ttu-id="363da-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="363da-135">The following is an example of the response.</span></span> 

><span data-ttu-id="363da-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="363da-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

<!-- uuid: A681726F-B4A7-4BCF-9407-F87CB9A4771D
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->