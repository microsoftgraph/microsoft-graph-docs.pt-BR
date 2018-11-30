---
title: Atualizar inferenceClassificationOverride
description: 'Alterar o campo **classifyAs** de uma caixa de entrada com foco substituir conforme especificado. '
ms.openlocfilehash: 696b3826bf09d3e0f706a3c3fdfba620e416ef22
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040211"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="b5728-103">Atualizar inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="b5728-103">Update inferenceClassificationOverride</span></span>

> <span data-ttu-id="b5728-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b5728-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5728-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b5728-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b5728-106">Alterar o campo **classifyAs** de uma [Caixa de entrada com foco](../resources/manage-focused-inbox.md) substituir conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="b5728-106">Change the **classifyAs** field of a [Focused Inbox](../resources/manage-focused-inbox.md) override as specified.</span></span> 

<span data-ttu-id="b5728-107">Você não pode usar PATCH para alterar outros campos em uma instância de [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="b5728-107">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span> 

<span data-ttu-id="b5728-108">Se houver uma substituição de um remetente e o remetente alterar seu nome de exibição, você poderá usar [POST](inferenceclassification-post-overrides.md) para forçar uma atualização para o campo de nome em uma substituição existente.</span><span class="sxs-lookup"><span data-stu-id="b5728-108">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="b5728-109">Se houver uma substituição de um remetente e o remetente alterar seu endereço SMTP, [excluir](inferenceclassificationoverride-delete.md) a substituição existente e [criar](inferenceclassification-post-overrides.md) uma nova com o novo endereço SMTP será a única maneira de "atualizar" a substituição deste remetente.</span><span class="sxs-lookup"><span data-stu-id="b5728-109">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5728-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5728-110">Permissions</span></span>
<span data-ttu-id="b5728-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5728-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5728-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5728-113">Permission type</span></span>      | <span data-ttu-id="b5728-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5728-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5728-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5728-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b5728-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5728-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b5728-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5728-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5728-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5728-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b5728-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5728-119">Application</span></span> | <span data-ttu-id="b5728-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5728-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5728-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5728-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b5728-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5728-122">Request headers</span></span>
| <span data-ttu-id="b5728-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b5728-123">Name</span></span>       | <span data-ttu-id="b5728-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5728-124">Type</span></span> | <span data-ttu-id="b5728-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5728-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b5728-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5728-126">Authorization</span></span>  | <span data-ttu-id="b5728-127">string</span><span class="sxs-lookup"><span data-stu-id="b5728-127">string</span></span>  | <span data-ttu-id="b5728-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5728-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b5728-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5728-130">Content-Type</span></span> | <span data-ttu-id="b5728-131">string</span><span class="sxs-lookup"><span data-stu-id="b5728-131">string</span></span>  | <span data-ttu-id="b5728-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5728-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5728-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5728-134">Request body</span></span>
<span data-ttu-id="b5728-p105">No corpo da solicitação, forneça o novo valor para **classifyAs**. Para obter o melhor desempenho, não inclua valores existentes que não estão sendo alterados.</span><span class="sxs-lookup"><span data-stu-id="b5728-p105">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="b5728-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5728-137">Property</span></span>     | <span data-ttu-id="b5728-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5728-138">Type</span></span>   |<span data-ttu-id="b5728-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5728-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5728-140">classifyAs</span><span class="sxs-lookup"><span data-stu-id="b5728-140">classifyAs</span></span>|<span data-ttu-id="b5728-141">string</span><span class="sxs-lookup"><span data-stu-id="b5728-141">string</span></span>| <span data-ttu-id="b5728-p106">Representa como classificar as mensagens recebidas de um remetente específico. Os valores possíveis são: `focused` e `other`.</span><span class="sxs-lookup"><span data-stu-id="b5728-p106">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="b5728-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5728-144">Response</span></span>

<span data-ttu-id="b5728-145">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5728-145">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5728-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5728-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5728-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5728-147">Request</span></span>
<span data-ttu-id="b5728-148">O exemplo a seguir altera a substituição para o endereço SMTP randiw@adatum.onmicrosoft.com de `other` para `focused`.</span><span class="sxs-lookup"><span data-stu-id="b5728-148">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
##### <a name="response"></a><span data-ttu-id="b5728-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5728-149">Response</span></span>
<span data-ttu-id="b5728-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5728-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Randi Welch",
    "address": "randiw@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->