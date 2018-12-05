---
title: Obter dataPolicyOperation
description: Recupere as propriedades do objeto dataPolicyOperation.
ms.openlocfilehash: fbc94719f9944adb25f7dd744cf0b15b179f3a5d
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2018
ms.locfileid: "27156016"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="94157-103">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="94157-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="94157-104">Recupere as propriedades do objeto dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="94157-104">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94157-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="94157-105">Permissions</span></span>
<span data-ttu-id="94157-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94157-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94157-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94157-108">Permission type</span></span>      | <span data-ttu-id="94157-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94157-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94157-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94157-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="94157-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94157-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="94157-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94157-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="94157-113">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="94157-113">Not applicable</span></span>  |
|<span data-ttu-id="94157-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94157-114">Application</span></span> | <span data-ttu-id="94157-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94157-115">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="94157-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94157-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="94157-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94157-117">Request headers</span></span>
| <span data-ttu-id="94157-118">Nome</span><span class="sxs-lookup"><span data-stu-id="94157-118">Name</span></span>      |<span data-ttu-id="94157-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="94157-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94157-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="94157-120">Authorization</span></span>  | <span data-ttu-id="94157-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="94157-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="94157-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94157-122">Request body</span></span>
<span data-ttu-id="94157-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94157-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="94157-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="94157-124">Response</span></span>
<span data-ttu-id="94157-125">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [dataPolicyOperation](../resources/datapolicyoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94157-125">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94157-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94157-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94157-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94157-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="94157-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="94157-128">Response</span></span>
<span data-ttu-id="94157-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94157-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dataPolicyOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 212

{
  "completedDateTime": "datetime-value",
  "id": "id-value",
  "status": "status-value",
  "storageLocation": "storageLocation-value",
  "userId": "userId-value",
  "submittedDateTime": "datetime-value",
  "progress": "progress-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
