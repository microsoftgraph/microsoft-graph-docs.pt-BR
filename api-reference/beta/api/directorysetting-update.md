---
title: Atualizar uma configuração de diretório
description: Atualize as propriedades de um objeto de configuração do diretório específico.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: f1c4c4c408f287fe6bfcf84eed3599aa85e3afbe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843347"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="7f03a-103">Atualizar uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="7f03a-103">Update a directory setting</span></span>

> <span data-ttu-id="7f03a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7f03a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f03a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7f03a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f03a-106">Atualize as propriedades de um objeto de configuração do diretório específico.</span><span class="sxs-lookup"><span data-stu-id="7f03a-106">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="7f03a-107">**Observação**: A versão de /beta desse API é só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="7f03a-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="7f03a-108">A versão de /v1.0 desse API foi renomeada para *Atualizar groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="7f03a-108">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f03a-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="7f03a-109">Permissions</span></span>
<span data-ttu-id="7f03a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f03a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f03a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f03a-112">Permission type</span></span>      | <span data-ttu-id="7f03a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f03a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f03a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f03a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7f03a-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7f03a-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7f03a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f03a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f03a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f03a-117">Not supported.</span></span>    |
|<span data-ttu-id="7f03a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f03a-118">Application</span></span> | <span data-ttu-id="7f03a-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f03a-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f03a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f03a-120">HTTP request</span></span>
<span data-ttu-id="7f03a-121"><!-- { "blockType": "ignored" } -->Atualize a todo um locatário ou configuração específica de grupo.</span><span class="sxs-lookup"><span data-stu-id="7f03a-121"><!-- { "blockType": "ignored" } --> Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="7f03a-122">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="7f03a-122">Optional request headers</span></span>
| <span data-ttu-id="7f03a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="7f03a-123">Name</span></span>       | <span data-ttu-id="7f03a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f03a-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7f03a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f03a-125">Authorization</span></span>  | <span data-ttu-id="7f03a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f03a-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f03a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f03a-128">Request body</span></span>
<span data-ttu-id="7f03a-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="7f03a-129">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="7f03a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f03a-130">Property</span></span>     | <span data-ttu-id="7f03a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f03a-131">Type</span></span>   |<span data-ttu-id="7f03a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f03a-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7f03a-133">values</span><span class="sxs-lookup"><span data-stu-id="7f03a-133">values</span></span> | <span data-ttu-id="7f03a-134">settingValue</span><span class="sxs-lookup"><span data-stu-id="7f03a-134">settingValue</span></span> | <span data-ttu-id="7f03a-p105">O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="7f03a-p105">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="7f03a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f03a-138">Response</span></span>

<span data-ttu-id="7f03a-139">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="7f03a-139">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7f03a-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f03a-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f03a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f03a-141">Request</span></span>
<span data-ttu-id="7f03a-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f03a-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_directorysetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/settings/{id}
Content-type: application/json
Content-length: 178

{
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="7f03a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f03a-143">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update directorysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
