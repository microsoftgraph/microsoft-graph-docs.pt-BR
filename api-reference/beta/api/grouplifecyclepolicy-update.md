---
title: Atualizar groupLifecyclePolicy
description: Atualiza as propriedades de um objeto do tipo de recurso groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 5914f0047a591ba53b160ba988342c13f0741fd6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955958"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="f81a2-103">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f81a2-103">Update groupLifecyclePolicy</span></span>

> <span data-ttu-id="f81a2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f81a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f81a2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f81a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f81a2-106">Atualiza as propriedades de um objeto do [tipo de recurso groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f81a2-106">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f81a2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f81a2-107">Permissions</span></span>

<span data-ttu-id="f81a2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f81a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="f81a2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f81a2-110">Permission type</span></span>      | <span data-ttu-id="f81a2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f81a2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f81a2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f81a2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f81a2-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f81a2-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f81a2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f81a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f81a2-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f81a2-115">Not supported</span></span> |
|<span data-ttu-id="f81a2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f81a2-116">Application</span></span> | <span data-ttu-id="f81a2-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f81a2-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f81a2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f81a2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="f81a2-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="f81a2-119">Optional request headers</span></span>
| <span data-ttu-id="f81a2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f81a2-120">Name</span></span> | <span data-ttu-id="f81a2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f81a2-121">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="f81a2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f81a2-122">Authorization</span></span> | <span data-ttu-id="f81a2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f81a2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f81a2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f81a2-125">Content-Type</span></span>  | <span data-ttu-id="f81a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f81a2-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f81a2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f81a2-127">Request body</span></span>

<span data-ttu-id="f81a2-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f81a2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f81a2-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f81a2-131">Property</span></span> | <span data-ttu-id="f81a2-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f81a2-132">Type</span></span> | <span data-ttu-id="f81a2-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f81a2-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f81a2-134">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="f81a2-134">alternateNotificationEmails</span></span>|<span data-ttu-id="f81a2-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f81a2-135">String</span></span>| <span data-ttu-id="f81a2-136">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="f81a2-136">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="f81a2-137">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="f81a2-137">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="f81a2-138">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="f81a2-138">groupLifetimeInDays</span></span>|<span data-ttu-id="f81a2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f81a2-139">Int32</span></span>| <span data-ttu-id="f81a2-140">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="f81a2-140">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="f81a2-141">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="f81a2-141">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="f81a2-142">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="f81a2-142">managedGroupTypes</span></span>|<span data-ttu-id="f81a2-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f81a2-143">String</span></span>| <span data-ttu-id="f81a2-144">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="f81a2-144">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="f81a2-145">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="f81a2-145">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="f81a2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f81a2-146">Response</span></span>

<span data-ttu-id="f81a2-147">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f81a2-147">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f81a2-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f81a2-148">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f81a2-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f81a2-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 151

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="f81a2-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="f81a2-150">Response</span></span>
<span data-ttu-id="f81a2-151">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f81a2-151">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
