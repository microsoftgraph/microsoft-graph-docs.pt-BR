---
title: 'usuário: exportPersonalData'
description: Envia uma solicitação de operação de política de dados, feita por um administrador da empresa para exportar dados de um usuário organizacionais.
ms.openlocfilehash: aceab65992bde3092676a2bfa144498f07f06095
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039358"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="4c756-103">usuário: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="4c756-103">user: exportPersonalData</span></span>

<span data-ttu-id="4c756-104">Envia uma solicitação de operação de política de dados, feita por um administrador da empresa para exportar dados de um usuário organizacionais.</span><span class="sxs-lookup"><span data-stu-id="4c756-104">Submits a data policy operation request, made by a Company Administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c756-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="4c756-105">Permissions</span></span>
<span data-ttu-id="4c756-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c756-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c756-108">Permission type</span></span>      | <span data-ttu-id="4c756-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c756-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c756-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c756-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4c756-111">User.Export.All</span><span class="sxs-lookup"><span data-stu-id="4c756-111">User.Export.All</span></span>  |
|<span data-ttu-id="4c756-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c756-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4c756-113">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="4c756-113">Not applicable</span></span>  |
|<span data-ttu-id="4c756-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c756-114">Application</span></span> | <span data-ttu-id="4c756-115">User.Export.All</span><span class="sxs-lookup"><span data-stu-id="4c756-115">User.Export.All</span></span> |

><span data-ttu-id="4c756-116">Observação: Export só pode ser executada por um administrador da empresa ao usar a permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="4c756-116">Note: Export can only be performed by a Company Administrator when using the delegated permission.</span></span>

## <a name="http-request"></a><span data-ttu-id="4c756-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c756-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="4c756-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c756-118">Request headers</span></span>
| <span data-ttu-id="4c756-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4c756-119">Name</span></span>       | <span data-ttu-id="4c756-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c756-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4c756-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c756-121">Authorization</span></span>  | <span data-ttu-id="4c756-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="4c756-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c756-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c756-123">Request body</span></span>
<span data-ttu-id="4c756-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c756-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4c756-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4c756-125">Parameter</span></span>    | <span data-ttu-id="4c756-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c756-126">Type</span></span>   |<span data-ttu-id="4c756-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c756-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c756-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="4c756-128">storageLocation</span></span>|<span data-ttu-id="4c756-129">String</span><span class="sxs-lookup"><span data-stu-id="4c756-129">String</span></span>|<span data-ttu-id="4c756-130">Esta é uma URL de assinatura (SAS) de acesso compartilhado para uma conta de armazenamento do Azure, para onde os dados devem ser exportados.</span><span class="sxs-lookup"><span data-stu-id="4c756-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="4c756-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c756-131">Response</span></span>
<span data-ttu-id="4c756-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c756-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c756-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c756-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c756-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c756-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```

##### <a name="response"></a><span data-ttu-id="4c756-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c756-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
