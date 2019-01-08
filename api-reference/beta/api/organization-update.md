---
title: Atualize a organização
description: Atualize as propriedades da organização autenticada no momento.
ms.openlocfilehash: a7b9521ccd39cb7cb64236c7d563a8a5c08d64a3
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748560"
---
# <a name="update-organization"></a><span data-ttu-id="96c7a-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="96c7a-103">Update organization</span></span>

> <span data-ttu-id="96c7a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="96c7a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96c7a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="96c7a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96c7a-106">Atualize as propriedades da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="96c7a-106">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="96c7a-107">Nesse caso, `organization` é definido como uma coleção de exatamente um registro, e, portanto, sua **ID** deve ser especificado na solicitação.</span><span class="sxs-lookup"><span data-stu-id="96c7a-107">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="96c7a-108">A **ID** é também conhecido como a **tenantId** da organização.</span><span class="sxs-lookup"><span data-stu-id="96c7a-108">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="96c7a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="96c7a-109">Permissions</span></span>

<span data-ttu-id="96c7a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96c7a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96c7a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96c7a-112">Permission type</span></span> | <span data-ttu-id="96c7a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96c7a-113">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96c7a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96c7a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="96c7a-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="96c7a-115">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="96c7a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96c7a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96c7a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96c7a-117">Not supported.</span></span> |
|<span data-ttu-id="96c7a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96c7a-118">Application</span></span> | <span data-ttu-id="96c7a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96c7a-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96c7a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96c7a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="96c7a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96c7a-121">Request headers</span></span>

| <span data-ttu-id="96c7a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="96c7a-122">Name</span></span>       | <span data-ttu-id="96c7a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="96c7a-123">Type</span></span> | <span data-ttu-id="96c7a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="96c7a-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="96c7a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="96c7a-125">Authorization</span></span>  | <span data-ttu-id="96c7a-126">string</span><span class="sxs-lookup"><span data-stu-id="96c7a-126">string</span></span>  | <span data-ttu-id="96c7a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96c7a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96c7a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96c7a-129">Request body</span></span>

<span data-ttu-id="96c7a-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="96c7a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="96c7a-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96c7a-133">Property</span></span>     | <span data-ttu-id="96c7a-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="96c7a-134">Type</span></span>   |<span data-ttu-id="96c7a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="96c7a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96c7a-136">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="96c7a-136">marketingNotificationEmails</span></span>|<span data-ttu-id="96c7a-137">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96c7a-137">String collection</span></span>|                                        <span data-ttu-id="96c7a-138">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="96c7a-138">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="96c7a-139">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="96c7a-139">privacyProfile</span></span>|[<span data-ttu-id="96c7a-140">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="96c7a-140">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="96c7a-141">O perfil de privacidade de uma organização (definir statementUrl e contactEmail).</span><span class="sxs-lookup"><span data-stu-id="96c7a-141">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="96c7a-142">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="96c7a-142">securityComplianceNotificationMails</span></span>|<span data-ttu-id="96c7a-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="96c7a-143">String collection</span></span>||
|<span data-ttu-id="96c7a-144">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="96c7a-144">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="96c7a-145">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96c7a-145">String collection</span></span>||
|<span data-ttu-id="96c7a-146">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="96c7a-146">technicalNotificationMails</span></span>|<span data-ttu-id="96c7a-147">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96c7a-147">String collection</span></span>|                                        <span data-ttu-id="96c7a-148">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="96c7a-148">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="96c7a-149">Desde que o recurso de **organização** oferece suporte às [extensões](/graph/extensibility-overview), você pode usar o `PATCH` operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância existente da **organização** .</span><span class="sxs-lookup"><span data-stu-id="96c7a-149">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="96c7a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="96c7a-150">Response</span></span>

<span data-ttu-id="96c7a-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96c7a-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96c7a-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96c7a-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96c7a-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96c7a-154">Request</span></span>
<span data-ttu-id="96c7a-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96c7a-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{id}
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

##### <a name="response"></a><span data-ttu-id="96c7a-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="96c7a-156">Response</span></span>

<span data-ttu-id="96c7a-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96c7a-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="96c7a-158">Confira também</span><span class="sxs-lookup"><span data-stu-id="96c7a-158">See also</span></span>

- [<span data-ttu-id="96c7a-159">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="96c7a-159">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="96c7a-160">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="96c7a-160">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
