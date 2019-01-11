---
title: Criar inferenceClassificationOverride
description: 'Crie uma substituição de caixa de entrada com foco de um remetente identificado por um endereço SMTP. As mensagens futuras desse endereço SMTP serão classificadas consistentemente '
localization_priority: Normal
ms.openlocfilehash: 1bccea7a585b5b30681d3f71d20340fe146eb6c6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892411"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="a88c0-104">Criar inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="a88c0-104">Create inferenceClassificationOverride</span></span>

> <span data-ttu-id="a88c0-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a88c0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a88c0-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a88c0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a88c0-107">Crie uma substituição de [Caixa de entrada com foco](../resources/manage-focused-inbox.md) de um remetente identificado por um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="a88c0-107">Create a [Focused Inbox](../resources/manage-focused-inbox.md) override for a sender identified by an SMTP address.</span></span> <span data-ttu-id="a88c0-108">Mensagens futura do que o endereço de SMTP será classificado consistentemente conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="a88c0-108">Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="a88c0-109">**Observação**</span><span class="sxs-lookup"><span data-stu-id="a88c0-109">**Note**</span></span>

- <span data-ttu-id="a88c0-110">Se já existir uma substituição com o mesmo endereço STMP, os campos **classifyAs** e **name** da substituição serão atualizados com os valores fornecidos.</span><span class="sxs-lookup"><span data-stu-id="a88c0-110">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="a88c0-111">O número máximo de substituições com suporte para uma caixa de correio é 1000, com base nos endereços SMTP exclusivos do remetente.</span><span class="sxs-lookup"><span data-stu-id="a88c0-111">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="a88c0-112">A operação POST dá suporte à criação de apenas uma substituição de cada vez.</span><span class="sxs-lookup"><span data-stu-id="a88c0-112">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="a88c0-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="a88c0-113">Permissions</span></span>
<span data-ttu-id="a88c0-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a88c0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a88c0-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a88c0-116">Permission type</span></span>      | <span data-ttu-id="a88c0-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a88c0-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a88c0-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a88c0-118">Delegated (work or school account)</span></span> | <span data-ttu-id="a88c0-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a88c0-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a88c0-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a88c0-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a88c0-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a88c0-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a88c0-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a88c0-122">Application</span></span> | <span data-ttu-id="a88c0-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a88c0-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a88c0-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a88c0-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="a88c0-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a88c0-125">Request headers</span></span>
| <span data-ttu-id="a88c0-126">Nome</span><span class="sxs-lookup"><span data-stu-id="a88c0-126">Name</span></span>       | <span data-ttu-id="a88c0-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a88c0-127">Type</span></span> | <span data-ttu-id="a88c0-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a88c0-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a88c0-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="a88c0-129">Authorization</span></span>  | <span data-ttu-id="a88c0-130">string</span><span class="sxs-lookup"><span data-stu-id="a88c0-130">string</span></span>  | <span data-ttu-id="a88c0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a88c0-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a88c0-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a88c0-133">Content-Type</span></span> | <span data-ttu-id="a88c0-134">string</span><span class="sxs-lookup"><span data-stu-id="a88c0-134">string</span></span>  | <span data-ttu-id="a88c0-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a88c0-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a88c0-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a88c0-137">Request body</span></span>
<span data-ttu-id="a88c0-138">No corpo da solicitação, forneça uma representação JSON do objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).</span><span class="sxs-lookup"><span data-stu-id="a88c0-138">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a88c0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a88c0-139">Response</span></span>

<span data-ttu-id="a88c0-140">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a88c0-140">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a88c0-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a88c0-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a88c0-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a88c0-142">Request</span></span>
<span data-ttu-id="a88c0-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a88c0-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/beta/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```

##### <a name="response"></a><span data-ttu-id="a88c0-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a88c0-144">Response</span></span>
<span data-ttu-id="a88c0-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a88c0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
