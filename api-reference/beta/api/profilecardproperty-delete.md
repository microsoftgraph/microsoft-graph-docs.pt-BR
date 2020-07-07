---
title: Excluir profileCardProperty
description: Exclua um objeto profileCardProperty e remova todas as personalizações do cartão de perfil.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c2dd6ef082167f40c173386f18be7760118a966f
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050997"
---
# <a name="delete-profilecardproperty"></a><span data-ttu-id="eff24-103">Excluir profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="eff24-103">Delete profileCardProperty</span></span>

<span data-ttu-id="eff24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eff24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eff24-105">Exclua o objeto [profileCardProperty](../resources/profilecardproperty.md) especificado por seu `directoryPropertyName` do cartão de perfil da organização e remova quaisquer personalizações localizadas para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="eff24-105">Delete the [profileCardProperty](../resources/profilecardproperty.md) object specified by its `directoryPropertyName` from the organization's profile card, and remove any localized customizations for that property.</span></span>

## <a name="permissions"></a><span data-ttu-id="eff24-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eff24-106">Permissions</span></span>

<span data-ttu-id="eff24-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="eff24-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="eff24-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eff24-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eff24-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eff24-109">Permission type</span></span>                        | <span data-ttu-id="eff24-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eff24-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eff24-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eff24-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eff24-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eff24-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="eff24-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eff24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eff24-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eff24-114">Not supported.</span></span>                              |
| <span data-ttu-id="eff24-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eff24-115">Application</span></span>                            | <span data-ttu-id="eff24-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eff24-116">Not supported.</span></span>                              |

><span data-ttu-id="eff24-117">**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="eff24-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="eff24-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eff24-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/organization/settings/profileCardProperties/{directoryPropertyName-Value}
```

## <a name="request-headers"></a><span data-ttu-id="eff24-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eff24-119">Request headers</span></span>

| <span data-ttu-id="eff24-120">Nome</span><span class="sxs-lookup"><span data-stu-id="eff24-120">Name</span></span>          | <span data-ttu-id="eff24-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eff24-121">Description</span></span>    |
|:--------------|:---------------|
| <span data-ttu-id="eff24-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eff24-122">Authorization</span></span> | <span data-ttu-id="eff24-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="eff24-123">Bearer {token}.</span></span> <span data-ttu-id="eff24-124">Required.</span><span class="sxs-lookup"><span data-stu-id="eff24-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eff24-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eff24-125">Request body</span></span>

<span data-ttu-id="eff24-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eff24-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eff24-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="eff24-127">Response</span></span>

<span data-ttu-id="eff24-128">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="eff24-128">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="eff24-129">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="eff24-129">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eff24-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eff24-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eff24-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eff24-131">Request</span></span>

<span data-ttu-id="eff24-132">O exemplo a seguir mostra como excluir o atributo chamado "fax" do cartão de perfil da organização.</span><span class="sxs-lookup"><span data-stu-id="eff24-132">The following example shows how to delete the attribute named "Fax" from the profile card for the organization.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_profilecardproperty"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/settings/profileCardProperties/fax
```

### <a name="response"></a><span data-ttu-id="eff24-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="eff24-133">Response</span></span>

<span data-ttu-id="eff24-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eff24-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
