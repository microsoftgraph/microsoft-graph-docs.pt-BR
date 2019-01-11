---
title: 'domínio: forceDelete'
description: Exclui um domínio usando uma operação assíncrona.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: e90b960bc2e2ff63068b1d91029371044075be27
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838056"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="64928-103">domínio: forceDelete</span><span class="sxs-lookup"><span data-stu-id="64928-103">domain: forceDelete</span></span>

> <span data-ttu-id="64928-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="64928-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64928-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="64928-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64928-106">Exclui um domínio usando uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="64928-106">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="64928-107">As seguintes ações são executadas como parte dessa operação:</span><span class="sxs-lookup"><span data-stu-id="64928-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="64928-108">Renomeia o UPN, EmailAddress e ProxyAddress de usuários com referências ao domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="64928-108">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="64928-109">Renomeia os EmailAddress dos grupos com referências ao domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="64928-109">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="64928-110">Renomeia o identifierUris de aplicativos com referências ao domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="64928-110">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="64928-111">Se o número de objetos a ser renomeado for maior que 1000, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="64928-111">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="64928-112">Se nenhum dos aplicativos a ser renomeado é um aplicativo de multilocatário, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="64928-112">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="64928-113">Após a exclusão de domínio for concluído, as operações de API para o domínio excluído retornará um código de resposta HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="64928-113">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="64928-114">Para verificar a exclusão de um domínio, você pode executar um [domínio de obter](domain-get.md).</span><span class="sxs-lookup"><span data-stu-id="64928-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="64928-115">Se o domínio foi excluído com êxito, será retornado um código de resposta HTTP 404 na resposta.</span><span class="sxs-lookup"><span data-stu-id="64928-115">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="64928-116">Permissions</span><span class="sxs-lookup"><span data-stu-id="64928-116">Permissions</span></span>

<span data-ttu-id="64928-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64928-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="64928-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64928-119">Permission type</span></span>      | <span data-ttu-id="64928-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64928-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64928-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64928-121">Delegated (work or school account)</span></span> | <span data-ttu-id="64928-122">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64928-122">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64928-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64928-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64928-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64928-124">Not supported.</span></span>    |
|<span data-ttu-id="64928-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64928-125">Application</span></span> | <span data-ttu-id="64928-126">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64928-126">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64928-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64928-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="64928-128">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="64928-128">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64928-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64928-129">Request headers</span></span>

| <span data-ttu-id="64928-130">Nome</span><span class="sxs-lookup"><span data-stu-id="64928-130">Name</span></span>       | <span data-ttu-id="64928-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="64928-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="64928-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="64928-132">Authorization</span></span>  | <span data-ttu-id="64928-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64928-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="64928-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64928-135">Content-Type</span></span>  | <span data-ttu-id="64928-136">application/json</span><span class="sxs-lookup"><span data-stu-id="64928-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="64928-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64928-137">Request body</span></span>

<span data-ttu-id="64928-138">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64928-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="64928-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="64928-139">Parameter</span></span>    | <span data-ttu-id="64928-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="64928-140">Type</span></span>   |<span data-ttu-id="64928-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="64928-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64928-142">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="64928-142">disableUserAccounts</span></span>|<span data-ttu-id="64928-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="64928-143">Boolean</span></span>| <span data-ttu-id="64928-144">Opção para desabilitar contas de usuário renomeado.</span><span class="sxs-lookup"><span data-stu-id="64928-144">Option to disable renamed user accounts.</span></span> <span data-ttu-id="64928-145">Se uma conta de usuário estiver desabilitada, o usuário não poderão entrar.</span><span class="sxs-lookup"><span data-stu-id="64928-145">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="64928-146">*True* (padrão) - usuário renomeadas como parte desta operação de contas estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="64928-146">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="64928-147">*False* - contas de usuário renomeadas como parte desta operação não estejam desabilitados.</span><span class="sxs-lookup"><span data-stu-id="64928-147">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="64928-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="64928-148">Response</span></span>

<span data-ttu-id="64928-149">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="64928-149">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="64928-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64928-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64928-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64928-151">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="64928-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="64928-152">Response</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
