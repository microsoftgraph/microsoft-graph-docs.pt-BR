---
title: Excluir a diretiva
description: Exclua uma política.
localization_priority: Normal
ms.openlocfilehash: 66772865fdff5ebf4b111cae91e60b00707bf6a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875359"
---
# <a name="delete-policy"></a><span data-ttu-id="ecdca-103">Excluir a diretiva</span><span class="sxs-lookup"><span data-stu-id="ecdca-103">Delete Policy</span></span>

> <span data-ttu-id="ecdca-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ecdca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecdca-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ecdca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ecdca-106">Exclua uma [política](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="ecdca-106">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ecdca-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ecdca-107">Permissions</span></span>
<span data-ttu-id="ecdca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecdca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecdca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecdca-110">Permission type</span></span>      | <span data-ttu-id="ecdca-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ecdca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecdca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecdca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ecdca-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ecdca-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ecdca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecdca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecdca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecdca-115">Not supported.</span></span>    |
|<span data-ttu-id="ecdca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecdca-116">Application</span></span> | <span data-ttu-id="ecdca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecdca-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecdca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecdca-118">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ecdca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecdca-119">Request headers</span></span>
| <span data-ttu-id="ecdca-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ecdca-120">Name</span></span>       | <span data-ttu-id="ecdca-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecdca-121">Type</span></span> | <span data-ttu-id="ecdca-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecdca-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ecdca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecdca-123">Authorization</span></span>  | <span data-ttu-id="ecdca-124">string</span><span class="sxs-lookup"><span data-stu-id="ecdca-124">string</span></span>  | <span data-ttu-id="ecdca-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecdca-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecdca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecdca-127">Request body</span></span>
<span data-ttu-id="ecdca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ecdca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecdca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecdca-129">Response</span></span>

<span data-ttu-id="ecdca-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ecdca-130">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="ecdca-131">Se não houver êxito …</span><span class="sxs-lookup"><span data-stu-id="ecdca-131">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="ecdca-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecdca-132">Example</span></span>
<span data-ttu-id="ecdca-133">O exemplo a seguir exclui uma diretiva.</span><span class="sxs-lookup"><span data-stu-id="ecdca-133">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="ecdca-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecdca-134">Request</span></span>
<span data-ttu-id="ecdca-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecdca-135">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="ecdca-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecdca-136">Response</span></span>
<span data-ttu-id="ecdca-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecdca-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
