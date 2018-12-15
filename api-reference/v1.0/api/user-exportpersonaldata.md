---
title: 'usuário: exportPersonalData'
description: Envia uma solicitação de operação de política de dados, feita por um administrador da empresa para exportar dados de um usuário organizacionais.
ms.openlocfilehash: 7d41d6d855fee992a4ff3a542e6c11f692adcfe3
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2018
ms.locfileid: "27284130"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="20651-103">usuário: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="20651-103">user: exportPersonalData</span></span>

<span data-ttu-id="20651-104">Envie uma solicitação de operação de política de dados de um administrador da empresa ou de um aplicativo para exportar dados de um usuário organizacional.</span><span class="sxs-lookup"><span data-stu-id="20651-104">Submit a data policy operation request from a company administrator or an application to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="20651-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="20651-105">Permissions</span></span>
<span data-ttu-id="20651-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20651-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20651-108">Permission type</span></span>      | <span data-ttu-id="20651-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20651-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20651-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20651-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="20651-111">User.Export.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="20651-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="20651-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20651-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="20651-113">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="20651-113">Not applicable</span></span>  |
|<span data-ttu-id="20651-114">Application</span><span class="sxs-lookup"><span data-stu-id="20651-114">Application</span></span> | <span data-ttu-id="20651-115">User.Export.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="20651-115">User.Export.All, User.Read.All</span></span> |

><span data-ttu-id="20651-116">**Observação:** A exportação só pode ser executada por um administrador da empresa quando permissões delegadas são usadas.</span><span class="sxs-lookup"><span data-stu-id="20651-116">**Note:** The export can only be performed by a company administrator when delegated permissions are used.</span></span>

## <a name="http-request"></a><span data-ttu-id="20651-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20651-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="20651-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20651-118">Request headers</span></span>
| <span data-ttu-id="20651-119">Nome</span><span class="sxs-lookup"><span data-stu-id="20651-119">Name</span></span>       | <span data-ttu-id="20651-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="20651-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="20651-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="20651-121">Authorization</span></span>  | <span data-ttu-id="20651-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="20651-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="20651-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20651-123">Request body</span></span>
<span data-ttu-id="20651-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20651-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20651-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="20651-125">Parameter</span></span>    | <span data-ttu-id="20651-126">Type</span><span class="sxs-lookup"><span data-stu-id="20651-126">Type</span></span>   |<span data-ttu-id="20651-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="20651-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20651-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="20651-128">storageLocation</span></span>|<span data-ttu-id="20651-129">String</span><span class="sxs-lookup"><span data-stu-id="20651-129">String</span></span>|<span data-ttu-id="20651-130">Esta é uma URL de assinatura (SAS) de acesso compartilhado para uma conta de armazenamento do Azure, para onde os dados devem ser exportados.</span><span class="sxs-lookup"><span data-stu-id="20651-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="20651-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="20651-131">Response</span></span>
<span data-ttu-id="20651-p102">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20651-p102">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20651-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20651-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20651-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20651-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```

##### <a name="response"></a><span data-ttu-id="20651-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="20651-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 202 Accepted
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
