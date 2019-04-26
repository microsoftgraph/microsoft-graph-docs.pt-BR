---
title: 'domínio: forceDelete'
description: Exclui um domínio usando uma operação assíncrona.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c58b7d345ba7c5cdc7c029ecf929676fc7529f12
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325864"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="874e2-103">domínio: forceDelete</span><span class="sxs-lookup"><span data-stu-id="874e2-103">domain: forceDelete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="874e2-104">Exclui um domínio usando uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="874e2-104">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="874e2-105">As ações a seguir são executadas como parte desta operação:</span><span class="sxs-lookup"><span data-stu-id="874e2-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="874e2-106">Renomeia o UPN, o EmailAddress e o ProxyAddress de usuários com referências para o domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="874e2-106">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="874e2-107">Renomeia o EmailAddress de grupos com referências para o domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="874e2-107">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="874e2-108">Renomeia a Identifieruris agora de aplicativos com referências para o domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="874e2-108">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="874e2-109">Se o número de objetos a serem renomeados for maior que 1000, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="874e2-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="874e2-110">Se um dos aplicativos a ser renomeado for um aplicativo de vários locatários, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="874e2-110">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="874e2-111">Após a conclusão da exclusão do domínio, as operações de API para o domínio excluído retornarão um código de resposta HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="874e2-111">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="874e2-112">Para verificar a exclusão de um domínio, você pode executar um [domínio Get](domain-get.md).</span><span class="sxs-lookup"><span data-stu-id="874e2-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="874e2-113">Se o domínio tiver sido excluído com êxito, um código de resposta HTTP 404 será retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="874e2-113">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="874e2-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="874e2-114">Permissions</span></span>

<span data-ttu-id="874e2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="874e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="874e2-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="874e2-117">Permission type</span></span>      | <span data-ttu-id="874e2-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="874e2-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="874e2-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="874e2-119">Delegated (work or school account)</span></span> | <span data-ttu-id="874e2-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="874e2-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="874e2-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="874e2-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="874e2-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="874e2-122">Not supported.</span></span>    |
|<span data-ttu-id="874e2-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="874e2-123">Application</span></span> | <span data-ttu-id="874e2-124">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="874e2-124">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="874e2-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="874e2-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="874e2-126">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="874e2-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="874e2-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="874e2-127">Request headers</span></span>

| <span data-ttu-id="874e2-128">Nome</span><span class="sxs-lookup"><span data-stu-id="874e2-128">Name</span></span>       | <span data-ttu-id="874e2-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="874e2-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="874e2-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="874e2-130">Authorization</span></span>  | <span data-ttu-id="874e2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="874e2-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="874e2-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="874e2-133">Content-Type</span></span>  | <span data-ttu-id="874e2-134">application/json</span><span class="sxs-lookup"><span data-stu-id="874e2-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="874e2-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="874e2-135">Request body</span></span>

<span data-ttu-id="874e2-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="874e2-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="874e2-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="874e2-137">Parameter</span></span>    | <span data-ttu-id="874e2-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="874e2-138">Type</span></span>   |<span data-ttu-id="874e2-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="874e2-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="874e2-140">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="874e2-140">disableUserAccounts</span></span>|<span data-ttu-id="874e2-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="874e2-141">Boolean</span></span>| <span data-ttu-id="874e2-142">Opção para desabilitar contas de usuário renomeadas.</span><span class="sxs-lookup"><span data-stu-id="874e2-142">Option to disable renamed user accounts.</span></span> <span data-ttu-id="874e2-143">Se uma conta de usuário estiver desabilitada, o usuário não terá permissão para entrar.</span><span class="sxs-lookup"><span data-stu-id="874e2-143">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="874e2-144">*True* (padrão)-as contas de usuário renomeadas como parte dessa operação estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="874e2-144">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="874e2-145">*False* -as contas de usuário renomeadas como parte dessa operação não estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="874e2-145">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="874e2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="874e2-146">Response</span></span>

<span data-ttu-id="874e2-147">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="874e2-147">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="874e2-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="874e2-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="874e2-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="874e2-149">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

##### <a name="response"></a><span data-ttu-id="874e2-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="874e2-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
